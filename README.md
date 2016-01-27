# vendorInternal
broken vendoring of golang.org/x/text/encoding/unicode

Vendored with 

```
govendor init
govendor add +external
``` 

Builds fine with `GO15VENDOREXPERIMENT=0`, but fails with `GO15VENDOREXPERIMENT=1`:

```
go run main.go
package golang.org/x/text/encoding/unicode
	imports golang.org/x/text/encoding/internal/identifier: use of internal package not allowed

```
