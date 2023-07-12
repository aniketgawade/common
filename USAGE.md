<!-- Start SDK Example Usage -->
```go
package main

import(
	"context"
	"log"
	"manager"
)

func main() {
    s := manager.New()

    ctx := context.Background()
    res, err := s.Common.DeleteAllCommonIntegrations(ctx)
    if err != nil {
        log.Fatal(err)
    }

    if res.ResponseMessage != nil {
        // handle response
    }
}
```
<!-- End SDK Example Usage -->