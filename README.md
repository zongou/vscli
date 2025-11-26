# VS Code Cli

Setting up runtime environment with PRoot and run vscode server.  
使用 PRoot 配置运行环境并运行 vscode 网页版。

## Server

Run a web version of vscode.  
运行 vscode 网页版。

```sh
./code serve-web \
  --host=0.0.0.0 \
  --port=8000 \
  --without-connection-token \
  "$@"
```

## Download

Download server.

```sh
./code download
```

## Patch

To work better on Android.  
为了更好的在 Android 上使用而打补丁。

```sh
./code patch
```

## Revert

Revert the patch.  
回退补丁。

```sh
./code revert
```
