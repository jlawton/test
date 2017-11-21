% GIT-RELEASE(1)
% James Lawton

# NAME

git-release(1) -- Create GitHub releases

# SYNOPSIS

**git release** [**-v** _version_] [_commit_]
**git release -h**

# DESCRIPTION

**git-release** creates a GitHub release from the current or given commit. It relies on the GitHub API, for which you must have a token configured. It is designed to be called by **git**, and is normally invoked as **git release**.

For detailed help, see **git release -h**.

# BASIC OPTIONS

**-a**
: Create an annotated tag, with the changelog as the message.

**-d** (**true**|**false**)
: If true, create a draft release.

**-h**
: Show detailed help.

**-v** _version_
: Force resolution to a specific version.

# CONFIGURATION

**git-release** uses a number of environment variables and git configurations. See detailed help for a full explanation.
