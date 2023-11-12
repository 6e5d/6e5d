# General info

* Projects are converted and mirrored from other VCS/server. Messages in github.com will not be replied.
* All projects will never have license files. The best way to reuse and share my code is to host it on tor/i2p.

# Build Instruction

Installation/configuration is a bad design.
Download projects and dependencies in `.lpat/deps.txt` (recursively) tn the same directory:

* Python: you need `importer.importer(relative_path, __FILE__)` function to locate relative library. It can be easily implemented with the builtin importlib.
* C: use [nomake](https://github.com/6e5d/nomake) project(usage: `nomake <project_root>`) that build all dependencies into shared library.
You may have to generate some missing files(e.g. by wayland-scanner, glslc) manually.
