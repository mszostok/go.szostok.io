# go.szostok.io

Go supports [vanity import paths](https://pkg.go.dev/cmd/go#hdr-Remote_import_paths) to decouple the import path and the code repository.

This repository holds sources for the [go.szostok.io](https://go.szostok.io) which is responsible for resolving `go get go.szostok.io/{name}` into `github.com/mszostok/{project}`.

## Build the site locally

Make sure you have installed [Hugo](https://gohugo.io) on your system. Follow the instructions to clone this repository and build the docs locally.

- Clone the repository

	```sh
	gh clone mszostok/go.szostok.io
	cd go.szostok.io
	```

- Fetch the theme submodule

	```sh
	git submodule update --init --recursive
	```

- Start local server

	```sh
	hugo serve -D
	```
	Site can be viewed at http://localhost:1313
