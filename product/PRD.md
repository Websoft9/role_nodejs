# Product requirement document

## Version

This role use [nvm](https://github.com/nvm-sh/nvm) to install Node, nvm is a version manager for node.js, designed to be installed per-user, and invoked per-shell. nvm works on any POSIX-compliant shell (sh, dash, ksh, zsh, bash), in particular on these platforms: unix, macOS, and windows WSL.

It can support v0.1.14 to latest, almost all version, and you can run command `nvm ls-remote` to list all version can be install

## Application

Some popular framework or application based on Node, you define it as application.  

This role should some application, e.g

* express
* @vue/cli
* @react/cli
