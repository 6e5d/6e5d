# General info

* Projects are converted and mirrored from other VCS/server. Use mail server(PORT 25, STARTTLS+PTR check required) for discussions.
* All projects do not have license files. The best way to reuse and share my code is to host it on tor/i2p.

# Build Instruction

Download projects and dependencies in `.lpat/deps.txt` recursively under the same directory.
All projects are designed to build and run in place. To achieve this some extra configurations are needed.

* Python: you need `importer.importer(relative_path, __FILE__)` function to locate relative library.

* C: use [nomake](https://github.com/6e5d/nomake) project(usage: `nomake <project_root>`) that build
all libraries to `/target/lib{name}.so` and all executables to `/target/{name}.elf`.

Note: some project require manually generated files(e.g. by `wayland-scanner`, `glslc`).
