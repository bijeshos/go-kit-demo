# Instructions

- `go build`
    - to build the project
- `./go-microservices`
    - to run the app
    - expected output: `msg=HTTP addr=:8080`
- In another terminal, to the following:
    - `curl -XPOST -d'{"s":"hello, world"}' localhost:8080/uppercase`
        - expected output: `{"v":"HELLO, WORLD"}`
    - `curl -XPOST -d'{"s":"hello, world"}' localhost:8080/count`
        - expected output: `{"v":12}`