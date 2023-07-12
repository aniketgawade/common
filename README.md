# manager

<!-- Start SDK Installation -->
## SDK Installation

```bash
go get github.com/speakeasy-sdks/common
```
<!-- End SDK Installation -->

## SDK Example Usage
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

<!-- Start SDK Available Operations -->
## Available Resources and Operations


### [Common](docs/sdks/common/README.md)

* [DeleteAllCommonIntegrations](docs/sdks/common/README.md#deleteallcommonintegrations) - Delete all common integrations
* [DeleteOneCommonIntegration](docs/sdks/common/README.md#deleteonecommonintegration) - Delete common integration
* [GetAllCommonIntegrations](docs/sdks/common/README.md#getallcommonintegrations) - Get all common integrations
* [GetOneCommonIntegration](docs/sdks/common/README.md#getonecommonintegration) - Get common integration
* [PostCommonIntegration](docs/sdks/common/README.md#postcommonintegration) - Create common integration
* [PutAllCommonIntegration](docs/sdks/common/README.md#putallcommonintegration) - Update common integration
<!-- End SDK Available Operations -->

### Maturity

This SDK is in beta, and there may be breaking changes between versions without a major version update. Therefore, we recommend pinning usage
to a specific package version. This way, you can install the same version each time without breaking changes unless you are intentionally
looking for the latest version.

### Contributions

While we value open-source contributions to this SDK, this library is generated programmatically.
Feel free to open a PR or a Github issue as a proof of concept and we'll do our best to include it in a future release!

### SDK Created by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/client-sdks)
