# Tools and Scripts

[gh](man/gh.1.md) [[source](bin/gh)] -- Open GitHub
[semver](man/semver.1.md) [[source](bin/semver)] -- Operate on Semantic Versions

## Installation

The easiest way to use these scripts is to add the `bin/` directory to your `PATH`.

You can also add the man pages, by compiling them and adding them to your `MANPATH`.

If you use Bash, for instance, you can do something like this from your working copy of this repository:

```
echo "export PATH=$PATH:$(pwd)/bin" >> ~/.bashrc

make -C man
echo "export MANPATH=$MANPATH:$(pwd)/man" >> ~/.bashrc
```
