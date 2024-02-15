<!-- Start SDK Example Usage [usage] -->
```go
package main

import (
	"context"
	testpetstore "github.com/speakeasy-sdks/test-petstore"
	"github.com/speakeasy-sdks/test-petstore/pkg/models/shared"
	"log"
	"net/http"
)

func main() {
	s := testpetstore.New()

	ctx := context.Background()
	res, err := s.Pets.CreatePets(ctx, shared.Pet{
		ID:   596804,
		Name: "<value>",
	})
	if err != nil {
		log.Fatal(err)
	}

	if res.StatusCode == http.StatusOK {
		// handle response
	}
}

```
<!-- End SDK Example Usage [usage] -->