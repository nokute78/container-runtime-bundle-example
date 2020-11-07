# container-runtime-bundle-example

An example of filesytem bundle of container runtime spec.

Refer to https://github.com/opencontainers/runtime-spec/blob/master/bundle.md

## Build and Run with runc

```
$ go build hello.go
$ mv hello bundle/rootfs/
$ sudo runc create test -b bundle
$ sudo runc start test
hello world
```

## License

[Apache License v2.0](https://www.apache.org/licenses/LICENSE-2.0)