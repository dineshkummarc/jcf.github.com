---
layout: post
title: "Spoofing Remote Addresses in Tests"
date: 2012-03-30 15:28
comments: true
categories: Ruby, Rails
---

In the process of testing some custom error handling I found myself
needing to fake my remote address in order to bypass
`consider_all_requests_local`.

To do this with Capybara, and Rack::Test you can use the following
Cucumber step.

``` ruby
Given /^I send requests from a remote address$/ do
  page.driver.browser.current_session.instance_eval {
    @headers['REMOTE_ADDR'] = '10.0.1.1'
  }
end
```

The reason this is necessary is that Rack::Test does not expose
the `REMOTE_ADDR` header, instead always setting the value to 127.0.0.1.

<!-- more -->

``` ruby
def default_env
  { "rack.test" => true, "REMOTE_ADDR" => "127.0.0.1" }.merge(headers_for_env)
end

def headers_for_env
  converted_headers = {}

  @headers.each do |name, value|
    env_key = name.upcase.gsub("-", "_")
    env_key = "HTTP_" + env_key unless "CONTENT_TYPE" == env_key
    converted_headers[env_key] = value
  end

  converted_headers
end
```

- [404s in Rails 3][]
- [Alex Rothenberg][]
- [Rack::Test#default_env][]

[404s in Rails 3]: https://github.com/rails/rails/issues/671#issuecomment-1780159
[Alex Rothenberg]: http://www.alexrothenberg.com/2011/11/21/testing-ip-whitelisting-in-your-specs-and-features.html
[Rack::Test#default_env]: https://github.com/brynary/rack-test/blob/fa7c6f9baf06e13352b42887e96c15c69bc10cb2/lib/rack/test.rb#L271
