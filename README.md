# API-Mathpix

A Perl module to use the Mathpix API

# Installation

To install this module, run the following commands:

	perl Makefile.PL
	make
	make test
	make install

# Usage

    my $mathpix = API::Mathpix->new({
      app_id  => $ENV{MATHPIX_APP_ID},
      app_key => $ENV{MATHPIX_APP_KEY},
    });

    my $response = $mathpix->process({
      src     => 'https://mathpix.com/examples/limit.jpg',
    });

    print $response->text; # your sweet LaTeX is there

# Licence and copyright

This software is Copyright (c) 2021 by Eriam Schaffter.

This is free software, licensed under:

  The Artistic License 2.0 (GPL Compatible)
