# Building

## Linux

### Ubuntu / Raspberry Pi OS

```shell
sudo apt install libgtk-3-dev libjavascriptcoregtk-4.1-dev libsoup-3.0-dev libwebkit2gtk-4.1-dev
```

## Run Dev Mode

```shell
cd modules/smearor
pnpm run tauri dev
```

## Build in Release Mode

```shell
cargo build --release
```
