# MiniProfiler Dashboard

A stupidly simple dashboard for `Rack::MiniProfiler`. It just implements a
better UI and makes it possible to profile non-html APIs too (which is my main
use-case)

# Install

`gem install miniprofiler-dashboard`

# Usage

In your `config.ru`:

```ruby
require 'rack-mini-profiler'
require 'rack/miniprofiler/dashboard'

map '/profiler' do
  use Rack::MiniProfiler::Dashboard
end
```

Then start the app and visit `/profiler`.

# TODO

  - Client-side stats
  - Bookmarklet?

# License

The MIT License (MIT)

Copyright (c) 2014 Luca Ongaro

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
