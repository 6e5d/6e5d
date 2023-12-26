Note: it seems that github may take down your account any time as long as they think it is not "secure".
My homepage mirror(of latest snapshot) is also available at <https://6e5d.com/lpat>.

* Projects are converted and mirrored from other VCS/server. Use mail server(PORT 25, STARTTLS+PTR check required) for discussions.
* All projects do not have license files. The best way to reuse and share my code is to host it on tor/i2p.

The build system is not stable yet. If you want to give it a try:

* first of all, all projects are designed to build and run in place. there is no configuration/installation/optional features, so the configuration is inherently trivial.
* `.lpat/deps.txt` specifies project dependencies.
* the `nomake` project should build c projects without any make system.
* for python projects, you should grep `importer`, where a global function is used to locate relative packages.
