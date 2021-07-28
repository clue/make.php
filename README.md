# clue/make.php

A GNU Make clone written in pure PHP. Run your Makefiles no matter whether GNU make is available.

**Table of contents**

* [Why?](#why)
* [Install](#install)
* [License](#license)

## Why?

GNU Make is a build automation tool that automatically builds (executable) programs
or libraries from source code by reading a `Makefile` which specifies how to derive the target program.
Besides building target programs, this is also often used to help automating
repetitive work, such as the program setup, test environment and build deployment.

Here's a simple `Makefile` with two build targets and a set of simple rules:

```makefile
build:
	@echo -n .
	@sleep 1
	@echo -n .
	@sleep 1
	@echo -n .
	@sleep 1
	@echo OK

test:
	vendor/bin/phpunit
```

If you have GNU Make installed, you can simply execute the first target like this:

```bash
$ make build
...OK
```

However, not every system has GNU Make installed (think Docker containers, shared hosting, Windows machines etc.).
That's where this project comes into play.

Once [installed](#install), you can simply execute the first target like this:

```bash
$ php vendor/bin/make.php build
...OK
```

You can reuse your existing `Makefile` without switching to a different build script language.
Or in other words: *Run your Makefiles no matter whether GNU make is available.*

## Install

[![A clue·access project](https://raw.githubusercontent.com/clue-access/clue-access/main/clue-access.png)](https://github.com/clue-access/clue-access)

*This project is currently under active development,
you're looking at a temporary placeholder repository.*

The code is available in early access to my sponsors here: https://github.com/clue-access/make.php

Do you sponsor me on GitHub? Thank you for supporting sustainable open-source, you're awesome! ❤️ Have fun with the code! 🎉

Seeing a 404 (Not Found)? Sounds like you're not in the early access group. Consider becoming a [sponsor on GitHub](https://github.com/sponsors/clue) for early access. Check out [clue·access](https://github.com/clue-access/clue-access) for more details.

This way, more people get a chance to take a look at the code before the public release.

Rock on 🤘

## License

This project will be released under the permissive [MIT license](LICENSE).

> Did you know that I offer custom development services and issuing invoices for
  sponsorships of releases and for contributions? Contact me (@clue) for details.
