# Generate all possibilities based on regularity

* [English](./README.md)
* [简体中文](./README_cn.md)

## Usage

```
Usage of crun:
           crun <regexp>
        or crun "\d{3}"
        or crun "[0-9a-z]{2}"
        or crun "(root|admin) [0-9]{1}"
```


### Example

``` bash
# Generates a number of all possible combinations of 1 to 6 digits in length
crun "\d{1,6}"

# Violence aesthetics
crun "(root|admin):[0-9]{4,5}"

# Note: If the amount is too big super card
```

### Install
``` bash

# Set environment variables, if set, please ignore
mkdir -p $HOME/gopath
export GOPATH=$HOME/gopath
export GOBIN=$GOPATH/bin
export PATH=$GOBIN:$PATH

# Download & Install
go get -u -v github.com/wzshiming/crun/cmd/crun

```
