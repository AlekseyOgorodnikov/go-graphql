# graphql

go get `go get github.com/99designs/gqlgen`

go run `go run github.com/99designs/gqlgen init`

go get -u github.com/99designs/gqlgen/cmd

Create a new file called graph/schema.graphqls

At the top of our resolver.go, between package and import, add the following line:
`//go:generate go run github.com/99designs/gqlgen`

This magic comment tells go generate what command to run when we want to regenerate our code. To run go generate recursively over your entire project, use this command:

`go generate ./...`
