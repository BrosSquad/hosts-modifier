# hosts-modifier
> Hosts file manager

# Introduction

Hosts-modifier is a program that aims to help you manage the system hosts file (```/etc/hosts``` on linux and ```C:\Windows\system32\drivers\etc\hosts``` on Windows).
It simplifies the process of adding, removing and listing lines in the file.
(Adding and Removing require administrator or super user privileges in the console or terminal.)

This program is designed for developers to help them manage host files, which they often do. (PHP develpment with XAMPP or any LAMPP stack, Laravel, Blocking sites etc...).

# Installation

Arch Linux users can build the program from the AUR, here is an example using yay:
```sh
yay -S hosts-modifier
```

Currently the only supported methods of installation are building the program from source code or building the program from the AUR. (Don't worry, go build is simple and so is the AUR.)
**Make sure you have golang installed for your operating system**

```sh
go get github.com/BrosSquad/hosts/cmd/hosts
```
**Make sure you've added $GOPATH/bin to the $PATH**
That's all.

# Usage

> hosts-modifier is a command line program


#### Get Help

```sh
$ hosts --help
```

#### Add Host

```sh
$ hosts add example.com 127.0.0.1
```

- If you don't pass ip, defaults to "127.0.0.1" (same as example above)

```sh
$ hosts add example.com
```

#### Remove Host

```sh
$ hosts remove example.com
```

#### List Hosts

```sh
$ hosts list
```

## Licence

This program is licensed under the terms of the **GNU GPL v2** only.
