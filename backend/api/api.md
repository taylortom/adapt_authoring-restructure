# api

This folder will contain the public-facing API of the application. The majority of the code in here will be concerned with routing requests, the business logic will still be handled by the 'manager'/controller files in `lib` (to make sure we separate concerns properly, it may make sense to separate out the 'controller' code from `lib` into individual controller files, which could go into here too). I intend to use express 4 sub-routers to do this.

Depending on how much stuff we have related to individual APIs, the folder may contain sub-folders, or just a .js file for each api router.

```
e.g.
// just files
assetRoutes.js
userRoutes.js
// folders
asset/
  assetRoutes.js
  assetModel.js
  assetSchema.js
  assetController.js
  ... blah
user/
  userRoutes.js
...etc.
```
