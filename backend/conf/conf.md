# conf

I'd like to do more with this folder, as it's not all that useful at the moment. I think it would be useful to make a bit more of this, and create multiple levels of config (at least for each type of environment: dev, prod, test), and store all options in here. As it is we already have a testConfig.json in `test/` which should probably be in here.

We could also hook into `process.env.NODE_ENV` or something to set/determine this, and load the suitable file.

i.e.
```
require('./' + env);
```
