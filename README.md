This repo contains a demo Todo List app for
[caddy-xtemplates](https://github.com/infogulch/caddy-xtemplates), a
[Caddy](https://caddyserver.com) module that turns Go's html/template library
into a featured hypertext preprocessor.

# Setup

1. Download `caddy` with all standard modules, plus the `xtemplates` module (!important).
    * Download from Caddy's public build system: https://caddyserver.com/download?package=github.com%2Finfogulch%2Fcaddy-xtemplates
    * Alternatively, install [`xcaddy`](https://github.com/caddyserver/xcaddy) and build from source yourself:

        ```sh
        xcaddy build --with github.com/infogulch/caddy-xtemplates

        # build with CGO in order to use the sqlite3 db driver
        CGO_ENABLED=1 xcaddy build --with github.com/infogulch/caddy-xtemplates
        ```
2. Run `caddy --config Caddyfile` from the root of this repository
3. Open `http://localhost:8080`
