# Build Instruction

Installation/configuration is a bad design.
All projects here are designed to build and run in place.
Just download projects and dependencies in `.lpat/deps.txt` (recursively) in the same directory:

* For python projects, you need to implement a global `importer.importer(relative_path, __FILE__)` function to locate relative library. It can be easily implemented with the builtin importlib.
  
* For C projects, you can use the [nomake](https://github.com/6e5d/nomake) project(usage: `nomake <project_root>`) and it will automatically build all dependencies into shared library. You may have to generate some missing files(e.g. by wayland-scanner, glslc) manually. Hopefully everything will be handled automatically in the future.

# Projects

* Projects are converted from 6e5d.com/lpat VCS by 6e5d.com/gitcompat converted, and synced by 6e5d.com/com_code.
Messages in github.com will not be responded.

* All projects will never have license file. Making authorship information overhead of human knowledge is a bad idea.
The best way to reuse my code is to host it on tor/i2p.
