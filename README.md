# git-dclone

Clone git repository with consistent directory hierarchy:
* Provider
* Owner
* Repository name

## Usage

```shell
git dclone URL

URL supports SSH and HTTPS scheme.
The SRC_DIR environment variable sets the workspace directory name where repositories should be cloned.
```

### Example

```shell
$ git dclone https://github.com/maxgio92/git-dclone.git
...
$ tree -L 3 src 
src
└── github.com
    └── maxgio92
        └── git-dclone
```

## Install

```shell
git clone https://github.com/maxgio92/git-dclone.git
export PATH=$PATH:~/.git-dclone"
./git-dclone/install.sh
```

