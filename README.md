## Note:
This is a small spinoff of an R package used to generate grid layouts.
The main development happens over at [rstudio/gridlayout](https://github.com/rstudio/gridlayout).

# Running dev environment

Parcel is used for bundling up dependencies.


All commands are run from within the `www/` directory.

## Actively developing just for front-end:

``` bash
parcel index.html
```
This will give you a live-reload server.


## Building a "deployment" version of app

First generate a bundled javascript file without source-map bloat
```bash
parcel build index.ts --no-source-maps 
```

Then switch the script source to `dist/index.js` from `./index.ts` in `index.html`. 
