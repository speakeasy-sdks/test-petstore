<!-- Start SDK Example Usage -->


```go
package main

import(
	"context"
	"log"
	testpetstore "github.com/speakeasy-sdks/test-petstore"
)

func main() {
    s := testpetstore.New()

    ctx := context.Background()
    res, err := s.Pets.CreatePets(ctx)
    if err != nil {
        log.Fatal(err)
    }

    if res.StatusCode == http.StatusOK {
        // handle response
    }
}
```
<!-- End SDK Example Usage -->