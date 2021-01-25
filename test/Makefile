BIN_DIR ?= ../bin

all:
	GOOS=linux GOARCH=386 go build -o ${BIN_DIR}/test-linux test.go
	GOOS=windows GOARCH=386 go build -o ${BIN_DIR}/test-windows.exe test.go
