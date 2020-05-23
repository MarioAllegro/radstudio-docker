# radstudio-docker
RAD Studio docker images

# Usage

```Dockerfile
FROM magicxor/radstudio:10.1-delphi-net3.5-ltsc2019
SHELL ["powershell"]

COPY YourApp /build/app
WORKDIR /build/app
RUN msbuild /t:build YourApp.dproj;
```