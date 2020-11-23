# Demo Web Server Written in Golang

### Step 0. Check environment

```bash
go env
go env GOPATH
go env -w GO111MODULE=on
```

### Step 1. Init the Go Module
```bash
mkdir go-web-demo && cd go-web-demo
go mod init github.com/xilu-wang/go-web-demo
go get -u github.com/gin-gonic/gin

#### Common usage ####
go get <MODULE_PATH>@latest
go get <MODULE_PATH>@<TAG>
go get <MODULE_PATH>@<BRANCH>
go get <MODULE_PATH>@<COMMIT_HASH>
go get -u <MODULE_PATH> # update current dependency
go mod download # download all dependencies in go.mod
go mod tidy # clean up dependencies 
go mod graph
go mod vendor
go mod verify
```

### Step 2. Keywords in go.mod

[go.mod](src/go.mod)

- module
- go
- require 
- exclude
- replace