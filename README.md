Add this buildpack to your Heroku application to install the wkhtmltopdf and wkhtmltoimage binaries, and the corresponding library libwkhtmltox, into the dynos:

```
heroku buildpacks:add https://github.com/milopets/heroku-wkhtmltopdf-buildpack --index 1
```

If you want to use a wkhtmltopdf version other than the default set WKHTMLTOPDF_DOWNLOAD_URL:

```
heroku config:set WKHTMLTOPDF_DOWNLOAD_URL="https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.bionic_amd64.deb"
```

You can see all the releases here: https://github.com/wkhtmltopdf/wkhtmltopdf/releases/