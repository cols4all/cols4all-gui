The app is based on the code from `app/app.R`.
To update the app, run the following command in the R console:

```r
shinylive::export("app", "docs")
```

Run the app locally with:

```r
if (require(httpuv)) {
  httpuv::runStaticServer("docs")
}
```