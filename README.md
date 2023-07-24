This repo contains a demo Todo List app for
[caddy-xtemplates](https://github.com/infogulch/caddy-xtemplates), a
[Caddy](https://caddyserver.com) module that turns Go's html/template library
into a featured hypertext preprocessor.

# Setup

1. Download `caddy` with all standard modules, plus the `xtemplates` module (!important) and put the binary in your PATH.
    * Until it's added as an official module, install `xcaddy` and build with:

          CGO_ENABLED=1 xcaddy build --with github.com/infogulch/caddy-xtemplates

    * https://caddyserver.com/download?package=github.com%2Finfogulch%2Fcaddy-xtemplates
2. Run `caddy --config Caddyfile` from the root of this repository
3. Open `http://localhost:8080`
