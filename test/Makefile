BIN_DIR ?= ../bin

all:
	GOOS=linux GOARCH=386 go build -ldflags="-s -w" -o ${BIN_DIR}/test-linux test.go
	GOOS=windows GOARCH=386 go build -ldflags="-s -w" -o ${BIN_DIR}/test-windows.exe test.go
