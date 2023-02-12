# Logstash-exporter

Export metrics from Logstash to Prometheus.
The project was created as rewrite of existing awesome application
[logstash_exporter](https://github.com/BonnierNews/logstash_exporter),
which was also written in Go, but it was not maintained for a long time.
A lot of code was reused from the original project.

**This project is under development and is not ready for use.**

## Building

### Makefile

#### Available Commands

- `make all`: Builds binary executables for Linux, macOS, and Windows and saves them in the out directory.
- `make run`: Runs the Go Exporter application.
- `make build-<OS>`: Builds a binary executable for the specified OS (`<OS>` can be `linux`, `darwin`, or `windows`).
- `make clean`: Deletes all binary executables in the out directory.
- `make (default)`: Runs the Go Exporter application.

#### File Structure

The main Go Exporter application is located in the cmd/exporter/main.go file.
The binary executables are saved in the out directory.

#### Example Usage

Build binary executables for all supported operating systems:

    make all

Run the Go Exporter application:

    make run

Build a binary executable for macOS:

    make build-darwin

Delete all binary executables:

    make clean