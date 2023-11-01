<!-- Start SDK Example Usage -->


```go
package main

import (
	"context"
	testsamplesdk16 "github.com/speakeasy-sdks-dev/test-sample-sdk-16"
	"log"
)

func main() {
	s := testsamplesdk16.New()

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