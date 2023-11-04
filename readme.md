# Build Instruction

I don't like the idea of installation and configuration,
therefore all projects here are designed to build and run in place.
Just download projects and dependencies in `.lpat/deps.txt` (recursively) in the same directory:

* For python projects, you need to implement a global `importer.importer(relative_path, __FILE__)` function to locate relative library. It can be easily implemented with the builtin importlib.
  
* For C projects, you can use the [nomake](https://github.com/6e5d/nomake) project(usage: `nomake <project_root>`) and it will automatically build all dependencies into shared library. You may have to generate some missing files(e.g. by wayland-scanner, glslc) manually. Hopefully everything will be handled automatically in the future.
