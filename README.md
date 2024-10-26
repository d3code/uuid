# uuid
The uuid package generates and inspects UUIDs based on
[RFC 9562](https://datatracker.ietf.org/doc/html/rfc9562)
and DCE 1.1: Authentication and Security Services. 

This package builds upon the [github.com/google/uuid](https://github.com/google/uuid) library but makes a key modification: it changes the response type of `UUID().Value()` from `string` to `[]byte`.

This adjustment enables the use of UUIDs in databases that require a byte format rather than a string format, specifically serving as a replacement for the `uuid_to_bin` function in MySQL.

###### Install
```sh
go get github.com/d3code/uuid
```

###### Documentation 
[![Go Reference](https://pkg.go.dev/badge/github.com/google/uuid.svg)](https://pkg.go.dev/github.com/google/uuid)

Full `go doc` style documentation for the package can be viewed online without
installing this package by using the GoDoc site here: 
https://pkg.go.dev/github.com/d3code/uuid
