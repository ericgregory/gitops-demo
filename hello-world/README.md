# "Hello World" in Rust for wasmCloud

This is a simple Rust-based WebAssembly (Wasm) component intended to run on [wasmCloud](https://wasmcloud.com/), an Incubating project at the [Cloud Native Computing Foundation (CNCF)](https://www.cncf.io/) for running WebAssembly workloads in cloud-native environments. The component responds with a "Hello World" message for each request. 

## Contents

In addition to the standard elements of a Rust project, the template directory includes the following files and directories:

- `wit/`: Directory for WebAssembly Interface Type (WIT) packages that define interfaces
- `/manifests/`: Kubernetes CRD manifest for deploying a WebAssembly workload to wasmCloud

## Build Dependencies

Before starting, ensure that you have the following installed:

- [`cargo`](https://www.rust-lang.org/tools/install) 1.82+ for the Rust toolchain
- [Wasm Shell (`wash`)](https://github.com/wasmCloud/wash) for component development

### Developing with `wash`

Start a development loop:

```shell
wash dev
```

The component is accessible at localhost:8000. View the code and make changes in `src/lib.rs`.

### Clean Up

You can cancel the `wash dev` process with `Ctrl-C`.

## Building with `wash`

To build the component:

```shell
wash build
```

## Further Reading

To learn how to extend this example with additional capabilities, see the [Adding Capabilities](https://wasmcloud.com/docs/tour/adding-capabilities?lang=rust) section of the wasmCloud documentation.