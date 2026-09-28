# URLShort

A small Go URL shortener that redirects configured paths to target URLs.

## What this project does

- Maps short paths like `/urlshort` to full URLs
- Uses a fallback HTTP handler for unknown routes
- Supports redirect rules defined in YAML as well as an in-memory map

## Main components

- `main/main.go`: starts the HTTP server and defines example redirect mappings
- `handler.go`: contains the URL redirect logic, including `MapHandler` and `YAMLHandler`

## Run the app

```bash
go run ./main
```

Then visit one of the example routes in the server config, such as:

- `http://localhost:8080/urlshort`
- `http://localhost:8080/urlshort-godoc`

This project is a simple example of URL redirection in Go using path mappings and YAML-based configuration.
