# NAME

App::RemoteCommand - simple remote command launcher via ssh

# SYNOPSIS

    > rcommand [OPTIONS] HOSTS COMMANDS
    > rcommand [OPTIONS] --script SCRIPT HOSTS
    > rcommand [OPTIONS] --host-file FILE COMMANDS

# DESCRIPTION

App::RemoteCommand is a simple remote command launcher via ssh. The features are:

- execute remote command in parallel
- remember sudo password first, and never ask again
- you may specify a script file in local machine
- append hostname and time to each command output lines
- report success/fail summary

# CAVEATS

Currently this module assumes you can ssh the target hosts
without password or passphrase.
So if your ssh identity (ssh private key) requires a passphrase,
please use `ssh-agent`.

# LICENSE

Copyright (C) Shoichi Kaji.

This library is free software; you can redistribute it and/or modify it under the same terms as Perl itself.

# AUTHOR

Shoichi Kaji <skaji@cpan.org>
