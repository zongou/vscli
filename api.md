# code api

```sh
code serve-web --log trace --verbose
```

## Objects

```sh
set -eu
while IFS= read -r obj; do
if test "${obj:+1}"; then
    printf "%s: %s\n" ${obj} $(curl -Ss https://update.code.visualstudio.com/api/latest/${obj}/stable)
fi
done <<-EOF
web-standalone

server-linux-alpine-web
server-alpine-arm64-web
server-linux-legacy-x64-web
server-linux-arm64-web
server-linux-legacy-arm64-web
server-linux-armhf-web
server-linux-legacy-armhf-web
server-darwin-web
server-darwin-arm64-web
server-win32-web
server-win32-arm64-web

server-linux-alpine
server-alpine-arm64
server-linux-legacy-x64
server-linux-arm64
server-linux-legacy-arm64
server-linux-armhf
server-linux-legacy-armhf
server-darwin
server-darwin-arm64
server-win32
server-win32-arm64

cli-alpine-arm64
cli-alpine-x64
cli-darwin-arm64
cli-darwin-x64
cli-linux-arm64
cli-linux-armhf
cli-linux-x64
cli-win32-arm64
cli-win32-x64

darwin
darwin-arm64
darwin-universal

linux-arm64
linux-armhf
linux-deb-arm64
linux-deb-armhf
linux-deb-x64
linux-rpm-arm64
linux-rpm-armhf
linux-rpm-x64
linux-snap-x64
linux-x64

win32-arm64
win32-arm64-archive
win32-arm64-user
win32-x64
win32-x64-archive
win32-x64-user
EOF
```

## API

| API                                                                                                                           |
| ----------------------------------------------------------------------------------------------------------------------------- |
| https://update.code.visualstudio.com/api/releases/stable                                                                      |
| https://update.code.visualstudio.com/api/releases/insider                                                                     |
| https://update.code.visualstudio.com/api/commits/stable/server-linux-x64-web                                                  |
| https://update.code.visualstudio.com/api/latest/server-linux-x64-web/stable                                                   |
| https://update.code.visualstudio.com/api/update/server-linux-x64-web/stable/latest                                            |
| https://update.code.visualstudio.com/api/versions/1.106.3/server-linux-x64-web/stable                                         |
| https://update.code.visualstudio.com/api/versions/commit:bf9252a2fb45be6893dd8870c0bf37e2e1766d61/server-linux-x64-web/stable |

## Download

| Download                                                                                                     |
| ------------------------------------------------------------------------------------------------------------ |
| https://update.code.visualstudio.com/latest/server-linux-x64-web/stable                                      |
| https://update.code.visualstudio.com/1.106.3/server-linux-x64-web/stable                                     |
| https://update.code.visualstudio.com/commit:bf9252a2fb45be6893dd8870c0bf37e2e1766d61/server-linux-x64/stable |
