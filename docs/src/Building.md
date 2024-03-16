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

Keen users can opt into multi-threaded mode with the -Z threads option:

```shell
RUSTFLAGS="-Z threads=8" cargo build --release
```
