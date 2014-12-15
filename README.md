# upload

A lightweight tool for synchronizing local directories with remote ones using
[Rsync](http://rsync.samba.org/).

## Usage

Simply type `upload` in your project directory (or any of its subdirectories)
and it will synchronize with your remote directory. upload uses
`$HOME/.upload/maps` and `$HOME/.upload/excludes` to function. Both these files
can be edited using `$EDTIOR` with the commands `upload --edit-maps` (`upload
--em` for short) or `upload --edit-excludes` (`upload -ee` fort short).

### Example of maps file

    /Users/KevinSjoberg/code/my-project my-remote-server.dev:/var/www/my-project

### Example of excludes file

    .git
    tmp/cache

Looking for a way to integrate `upload` with your editor? Check out
[Integrating with your
editor](https://github.com/KevinSjoberg/upload/wiki/Integrating-with-your-editor)
in the wiki section.
