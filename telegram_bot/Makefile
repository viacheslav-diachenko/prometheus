VERSION = $(shell git describe --tags --abbrev=0)-$(shell git rev-parse --short HEAD)
TARGETOS = windows #darwin linux
TARGETARCH = amd64 # arm64 x86
WINARCH = $(PROCESSOR_ARCHITEW6432)

ifeq ($(WINARCH),AMD64)
	TARGETARCH=amd64
else ifeq ($(WINARCH),x86)
	TARGETARCH=x86
endif

format:
	gofmt -s -w ./

linux:	
	TARGETARCH = ${shell uname -m | sed 's/x86_64/amd64/' | sed 's/arm64/arm64/' | sed 's/aarch64/arm64/' | sed 's/i686/x86/'}
	CGO_ENABLED=0 GOOS=linux GOARCH=${TARGETARCH} go build -v -o telegram_bot -ldflags "-X="github.com/viacheslav-diachenko/prometheus/tree/main/telegram_bot/cmd.appVersion=${VERSION}

windows:
	set CGO_ENABLED=0 GOOS=windows GOARCH=${TARGETARCH} 
	go build -v -o telegram_bot.exe -ldflags "-X="github.com/viacheslav-diachenko/prometheus/tree/main/telegram_bot/cmd.appVersion=${VERSION}

macOS:
	TARGETARCH = ${shell uname -m | sed 's/x86_64/amd64/' | sed 's/arm64/arm64/' | sed 's/aarch64/arm64/' | sed 's/i686/x86/'}
	CGO_ENABLED=0 GOOS=darwin GOARCH=${$TARGETARCH} go build -v -o telegram_bot -ldflags "-X="github.com/viacheslav-diachenko/prometheus/tree/main/telegram_bot/cmd.appVersion=${VERSION}