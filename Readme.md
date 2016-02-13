# Git Data

## git data management and backup utility

Within a git repository subfolder, performs a data backup to remote directory
but keeps 'file structure' to have local symbolic links to data.

Files already in local .gitignore are ignored.

Local files are replaced by symbolic links, and ignored in git.

Ghost files (prefixed .) are created to be seen by other instances of the repo.

## Usage

   launch `git data --remote=$REMOTE` in a git subfolder, where remote is the remote git root (subfolders are created as remote if not exists) to initialize ; without `--remote` option to update.

## Missing features

* ghostize or not option
* ssh remote
* multiple backup destinations within subfolders
* solution for gitignore ?
* commit option
* does not delete remote files on local delete
* metadata management ? -> difficult in shell
