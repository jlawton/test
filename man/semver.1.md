% SEMVER(1)
% James Lawton

# NAME

semver(1) -- Operate on Semantic Versions

# SYNOPSIS

**semver** _version_ **incr** (**major**|**minor**|**patch**) \
**semver** _version_ **get** (**major**|**minor**|**patch**) \
**semver** _version_ **~>** _version2_

# DESCRIPTION

Operate on [Semantic Versions](https://semver.org). Get parts of a version, or calculate version increments, outputting to STDOUT. Compare versions, returning the result in the exit code.

# OPERATIONS

Operations print results to STDOUT.

**incr** : Increment part of a version.
**get** : Get part of a version.

# COMPARISONS

Version comparisons return their results in the exit code. Zero, if the comparison is true. One, if the comparison is false.

_a_ **==** _b_ : Version _a_ is equal to version _b_.

_a_ **!=** _b_ : Version _a_ is not equal to version _b_.

_a_ **>** _b_ : Version _a_ is greater than _b_.

_a_ **>=** _b_ : Version _a_ is greater than or equal to _b_.

_a_ **~>** _b_ : Version _a_ is compatible with version requirement _b_.

# EXAMPLES

```
semver 1.2.3 incr major
==> 1
```

```
semver 1.2.3 ~> 1.2.0
# True
```
