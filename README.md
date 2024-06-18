[![build](https://github.com/nightblue-io/vortex-proto/actions/workflows/main.yml/badge.svg)](https://github.com/nightblue-io/vortex-proto/actions/workflows/main.yml)

The folder `google/*` was cloned from [github.com/googleapis/api-common-protos](https://github.com/googleapis/api-common-protos). The folder `protoc-gen-openapiv2/*` was cloned from [github.com/grpc-ecosystem/grpc-gateway/protoc-gen-openapiv2](https://github.com/grpc-ecosystem/grpc-gateway).

Install the following tools to build locally:

* The [`protoc`](https://grpc.io/docs/protoc-installation/) compiler,
* The following compiler plugins:

```bash
$ go install google.golang.org/protobuf/cmd/protoc-gen-go@latest
$ go install google.golang.org/grpc/cmd/protoc-gen-go-grpc@latest
$ go install github.com/grpc-ecosystem/grpc-gateway/v2/protoc-gen-grpc-gateway@latest
$ go install github.com/grpc-ecosystem/grpc-gateway/v2/protoc-gen-openapiv2@latest
$ go install github.com/pseudomuto/protoc-gen-doc/cmd/protoc-gen-doc@latest
```

* The [`buf`](https://docs.buf.build/installation) tool.

Then run:

```bash
$ ./build.sh
```

Generated artifacts from this repository:

* https://github.com/nightblue-io/vortex-go/ - Go SDK
* https://nightblue-io.github.io/vortex-apidocs/ - OpenAPI docs
