# rgit - Remote GIT

rgit is a remote git utility to create a bare repository on a remote server.


`rgit` is useful if you want to create a repository on your on VPS without
manually `ssh`ing into it and creating a bare repo. `rgit` is POSIX complaint.


`rgit` will also try to set the remote (either "server" or `$REMOTE_ORIGIN`) of
the current repo (that is, from the directory `rgit` was invoked from) 

## Dependencies

- `git` `ssh`

## Usage

`rgit test/test.git`

## Configuration

Configuration of `rgit` is done via `source`ing a file at `~/.config/rgit.conf`

```sh 

# ~/.config/rgit.conf

# Example configuration provided. Refer to man page for more information.
DOMAIN=example.com USER=git GIT_DIR=/git 

```

## LICENSE

`rgit` is licensed under the GNU General Public License 3. Our copy of the
license can be found [here](./LICENSE)
