# QuickDuck

**This is a fork of [Unduck](https://github.com/t3dotgg/unduck)**

DuckDuckGo's bang redirects are too slow. Add the following URL as a custom search engine to your browser. Enables all of DuckDuckGo's bangs to work, but much faster.

```text
https://quickduck.vercel.app?q=%s
```

## How is it that much faster?

DuckDuckGo does their redirects server side. Their DNS is...not always great. Result is that it often takes ages.

Theo solved this by doing all of the work client side. Once you've went to [quickduck.vercel.app](https://quickduck.vercel.app) once, the JS is all cache'd and will never need to be downloaded again. Your device does the redirects, not the server.
