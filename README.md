[![Actions Status](https://github.com/p5-UV/Alien-libuv/workflows/linux/badge.svg)](https://github.com/p5-UV/Alien-libuv/actions)
[![Actions Status](https://github.com/p5-UV/Alien-libuv/workflows/macos/badge.svg)](https://github.com/p5-UV/Alien-libuv/actions)
[![Actions Status](https://github.com/p5-UV/Alien-libuv/workflows/windows/badge.svg)](https://github.com/p5-UV/Alien-libuv/actions)

# NAME

Alien::libuv - Interface to the libuv library [http://libuv.org](http://libuv.org)

# SYNOPSIS

In your `Makefile.PL`:

```perl
use strict;
use warnings;

use ExtUtils::MakeMaker;
use Config;
use Alien::Base::Wrapper ();

WriteMakefile(
  Alien::Base::Wrapper->new('Alien::libuv')->mm_args2(
    ...
    CONFIGURE_REQUIRES => {
      'Alien::libuv' => '1.000',
    },
    ...
  ),
);
```

# DESCRIPTION

This package can be used by other [CPAN](https://metacpan.org) modules that
require [libuv](http://libuv.org).

# AUTHOR

Chase Whitener <`capoeirab@cpan.org`>

# CONTRIBUTORS

Graham Ollis <`plicease@cpan.org`>

# COPYRIGHT & LICENSE

Copyright (c) 2017 Chase Whitener. All rights reserved.

This program is free software; you can redistribute it and/or modify it
under the same terms as Perl itself.
