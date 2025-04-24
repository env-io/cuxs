FROM qasico/go:latest

# Apps Dir
RUN mkdir -p "$GOPATH/src/github.com/env-io/cuxs/cuxs"
ADD . "$GOPATH/src/github.com/env-io/cuxs/cuxs"
WORKDIR "$GOPATH/src/github.com/env-io/cuxs/cuxs"

# Installing Dependency
RUN glide update

# Entry Point
ENTRYPOINT "$GOPATH/src/github.com/env-io/cuxs/cuxs"

CMD ["sleep","3600"]
