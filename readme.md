* I do not use git vcs. All projects here are mirrored by API and force pushed on update. So do not refer to any source code here (lines, revisions, etc.)
* All projects here are designed to build and run without installation, just download projects and dependencies in `.lpat/deps.txt` (recursively) in the same directory.
* For python projects you need to implement a global `importer.importer` function to locate relative library. It can be easily implemented with the builtin importlib.
