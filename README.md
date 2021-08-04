# Go Build Linker
This repository showcases how to use the -ldflags with the `go build` command to insert dynamic information into a binary at build time.

## Build the binary without ldflags
```
$ go build
$ ./go-build-linker 
Version: v0.1.0
```

## Build the binary and set the version to v1.0.0 using ldflags
```
$ go build -ldflags="-X 'main.Version=v1.0.0'"
$ ./go-build-linker
Version: v1.0.0
```
