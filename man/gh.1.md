% GH(1)
% James Lawton

# NAME

gh(1) -- Open GitHub

# SYNOPSIS

**gh** [_directory_] \
**gh** [**--format** _format_] [_directory_]

# DESCRIPTION

Open the GitHub or GitHub Enterprise repository page for the current or given working copy directory in the default browser.

It is assumed that current or given directory was cloned from GitHub, so `origin` will be a GitHub SSH or HTTPS address. If not, behavior is undefined.

# OPTIONS

**-f**, **--format** _format_
: Print parts of the GitHub URL, rather than opening a browser. _format_ can contain tags which will be replaced.

## Format Replacements

**:server**
: The host name. (eg. `github.com`)

**:owner**
: The repository owner.

**:repo**
: The repository name.

For instance, the default behavior of **gh** is equivalent to something like the following:

    open $(gh --format 'https://:server/:owner/:repo')
