# perl6-concurrent-file-find
[![Build Status](https://travis-ci.org/gfldex/perl6-concurrent-channelify.svg?branch=master)](https://travis-ci.org/gfldex/perl6-concurrent-channelify)

turn a lazy list into a auto-threading lazy list

# SYNOPSIS

```
use v6;
use Concurrent::Channelify;


```

# DESCRIPTION

## Routines

### sub channelify(Positional:D, :$no-thread = False)

Return a new lazy list that is turned into a `Channel`. If `no-thread` is
`True` do not start a thread to generate values. The environment variable
`RAKUDO_MAX_THREAD` with a value smaller then 2 has the same effect then
`no-thread`, if set before the use-statement is executed.

### postfix ⇒

