# blink1-run

> A tiny tool to hook up your blink(1) device to commands on your beloved shell.

blink1-run will execute any given command within your current shell and start with a slow strobe light as an load indicator. Upon completion it will flash in green or red depending on the return state of the executed command.

## Install

Most OS need you to be root (e.g. using `sudo`) to install a global npm package:

```sh
$ npm -g install blink1-run
```

blink1-run depends on [Node.js](http://nodejs.org/) and [npm](http://npmjs.org/). Tested with `node v4.2.0` and `npm v2.14.7`.

## Usage

Prepend the `blink1-run` or `b1` alias to your command. Hook up your blink(1) device and run:

```sh
$ b1 <your-command> <argument-1> <argument-2> ...
```

examples:

```sh
$ b1 sleep 5
```

```sh
$ b1 echo simple/single commands can be used without quotation marks
```

```sh
$ b1 "sleep 5 && echo very complex c0mmand && sleep 5"
```

```sh
$ b1 "mysql -u mysqluser -p my_database < huge_database_dump.sql"
```

```sh
$ b1 cat flash_red_if_this_file_does_not_exist
```

## Todo

* test more shells, commands and OS

## Support

Found a bug? Open an issue [here](https://github.com/thbaumbach/blink1-run/issues) on Github.

Wanna help? Submit a pull request or contact me.

Wanna tip me a beer? Use [Bitcoin](bitcoin:14pSD9AmuNhLDbGRXehxbhwzRSRrkpiAKg): 14pSD9AmuNhLDbGRXehxbhwzRSRrkpiAKg

## License

Copyright (c) 2015 Thomas Baumbach <tom@xolo.pw>

Licensed under the MIT License
