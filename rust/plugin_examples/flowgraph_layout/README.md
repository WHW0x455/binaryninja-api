# FlowGraph Layout Example

This example implements a simple data renderer for the Mach-O load command LC_UUID.
You can try the renderer by loading the `/bin/cat` binary from macOS.

We're implementing a functionality similar to the one described in the Python data renderer blog post: 
https://binary.ninja/2024/04/08/customizing-data-display.html.

## Building

```sh
# Build from the root directory (binaryninja-api)
cargo build -p example_flowgraph_layout
# Link binary on macOS
ln -sf $PWD/target/debug/libexample_data_renderer.dylib ~/Library/Application\ Support/Binary\ Ninja/plugins
```
