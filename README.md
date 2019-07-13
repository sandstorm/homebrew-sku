# sku 


## Developing

## Releasing new versions


### Prerequisites for releasing

1. ensure you have [goreleaser](https://goreleaser.com/) installed:

  ```bash
  brew install goreleaser/tap/goreleaser
  ```

2. Create a new token for goreleaser [in your GitHub settings](https://github.com/settings/tokens); select the `repo` scope.

3. put the just-created token into the file `~/.config/goreleaser/github_token`



### Doing the release

Testing a release:

```
goreleaser --snapshot --skip-publish --rm-dist --debug
```

Executing a release:

1. Commit all changes, create a new tag and push it.

```
git tag v0.9.0
```


## Legacy


sku context

sku context "set context"

## install

```
brew install glide
```

set the GOPATH in e.g. your ~/.zshrc

```
export GOPATH=/Users/USERNAME/src/go
```

restart your console and run

now clone or move this repo into your GOPATH e.g. `~/src/go/src/github.com/sandstorm` and change to this direcotory. Than run: 

```
glide update --strip-vendor
./build.sh
```

To run this command everywhere create a symlink
```
ln -s /Users/USERNAME/src/go/src/github.com/sandstorm/sku/sku /usr/local/bin/
```
