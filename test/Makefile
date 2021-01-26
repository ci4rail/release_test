BIN_DIR ?= ../bin
VERSION ?= $(shell git describe --tags --dirty --exact-match 2>/dev/null || git rev-parse --short HEAD)
GO_LDFLAGS = -ldflags "-s -w -X main.version=$(VERSION)"

all:
	GOOS=linux GOARCH=386 go build ${GO_LDFLAGS} -o ${BIN_DIR}/test-linux test.go
	GOOS=windows GOARCH=386 go build ${GO_LDFLAGS} -o ${BIN_DIR}/test-windows.exe test.go
