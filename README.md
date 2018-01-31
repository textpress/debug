# debug
Up-friendly `debug` clone

## Problem

By default `debug` [will log to stderr](https://www.npmjs.com/package/debug#output-streams), which makes `up` [treat them as errors](https://github.com/apex/up/issues/565).

While this might be resolved with an option, it might be worthwhile to wrap debug regardless along the lines of https://www.npmjs.com/package/debug-levels to allow for a better granularity than "all or nothing".
