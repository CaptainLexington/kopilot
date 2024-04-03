**NOTE: This README is currently ✨ _aspirational._ ✨ I am describing the program I intend to write. Until this note is removed, assume it is basically nonfunctional.**

The sync server is forked from [kosync](https://github.com/lzyor/kosync).

# KOPilot Sidecar Management Server

KOPilot is a Sidecar Management Server for KOReader. KOReader's Sidecar files track reading metadata like progress, highlights, and notes. These can be synced between devices using a server provided at [koreader.rocks](koreader.rocks), but it is also possible to configure a custom server at a custom URL. KOPilot provides two servers: on one port it provides the kosync server for syncing sidecars between libraries, and on another it provides an HTTP server that allows you to browse Sidecar files and export their contents to a variety of formats. This means your highlights are accessible not only on all of your devices, but also on your personal server (and anywhere you can access it).



```bash
KOSYNC_ADDR=0.0.0.0:3000 ./kosync
```

## docker

```bash
docker pull lzyorstudio/kosync
```

## build

for linux

```bash
cargo build --release --target x86_64-unknown-linux-musl
```

for docker

```bash
./docker/make.sh
```

## WIP
