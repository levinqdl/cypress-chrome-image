# Build cypress docker image with specify chrome version

You can use this Dockerfile to build a image for CI on linux environment.

## How to use

1. download specific chrome package and put it in the directory

You can download chrome package from [here](http://170.210.201.179/linux/chrome/deb/pool/main/g/google-chrome-stable/).

2. build docker image

``` shell
docker build [--platform=amd64] --build-arg CHROME_VERSION=<chrome-version> . -t <your-tag>
```
'chrome version' should be same with package name
