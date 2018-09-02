# Coverage lines

Simple tool to get covered and total lines which might be useful if you're trying to calculate total coverage for multiple projects, some of which are not written in Go.

Please see [example](https://github.com/yb172/collider) for more context.

## Installation

Same as for any other go binary:

```bash
go get -u github.com/yb172/coverage-lines
```

## Usage

First run test with `-coverprofile` option enabled:

```bash
go test ./... -coverprofile=cover.out
```

And then run `coverage-lines`:

```bash
coverage-lines cover.out
```

It will output two numbers: number of covered statements and total number of statements
