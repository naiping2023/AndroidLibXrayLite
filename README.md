# AndroidLibXrayLite

## Build requirements
* JDK
* Android SDK
* Go
* gomobile

## Install gomobile
1. `go install golang.org/x/mobile/cmd/gomobile@latest`
2. `echo 'export PATH=~/go/bin:$PATH' >>~/.bash_profile`


## Build instructions
1. `git clone [repo] && cd AndroidLibXrayLite`
2. `gomobile init`
3. `go mod tidy -v`
4. `gomobile bind -v -androidapi 21 -ldflags='-s -w' ./`