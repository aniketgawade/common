# Common

### Available Operations

* [DeleteAllCommonIntegrations](#deleteallcommonintegrations) - Delete all common integrations
* [DeleteOneCommonIntegration](#deleteonecommonintegration) - Delete common integration
* [GetAllCommonIntegrations](#getallcommonintegrations) - Get all common integrations
* [GetOneCommonIntegration](#getonecommonintegration) - Get common integration
* [PostCommonIntegration](#postcommonintegration) - Create common integration
* [PutAllCommonIntegration](#putallcommonintegration) - Update common integration

## DeleteAllCommonIntegrations

Delete all common integrations

### Example Usage

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

### Parameters

| Parameter                                             | Type                                                  | Required                                              | Description                                           |
| ----------------------------------------------------- | ----------------------------------------------------- | ----------------------------------------------------- | ----------------------------------------------------- |
| `ctx`                                                 | [context.Context](https://pkg.go.dev/context#Context) | :heavy_check_mark:                                    | The context to use for the request.                   |


### Response

**[*operations.DeleteAllCommonIntegrationsResponse](../../models/operations/deleteallcommonintegrationsresponse.md), error**


## DeleteOneCommonIntegration

Delete common integration

### Example Usage

```go
package main

import(
	"context"
	"log"
	"manager"
	"manager/pkg/models/operations"
)

func main() {
    s := manager.New()

    ctx := context.Background()
    res, err := s.Common.DeleteOneCommonIntegration(ctx, operations.DeleteOneCommonIntegrationRequest{
        Name: "Terrence Rau",
    })
    if err != nil {
        log.Fatal(err)
    }

    if res.ResponseMessage != nil {
        // handle response
    }
}
```

### Parameters

| Parameter                                                                                                    | Type                                                                                                         | Required                                                                                                     | Description                                                                                                  |
| ------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------ |
| `ctx`                                                                                                        | [context.Context](https://pkg.go.dev/context#Context)                                                        | :heavy_check_mark:                                                                                           | The context to use for the request.                                                                          |
| `request`                                                                                                    | [operations.DeleteOneCommonIntegrationRequest](../../models/operations/deleteonecommonintegrationrequest.md) | :heavy_check_mark:                                                                                           | The request object to use for the request.                                                                   |


### Response

**[*operations.DeleteOneCommonIntegrationResponse](../../models/operations/deleteonecommonintegrationresponse.md), error**


## GetAllCommonIntegrations

Get all common integrations

### Example Usage

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
    res, err := s.Common.GetAllCommonIntegrations(ctx)
    if err != nil {
        log.Fatal(err)
    }

    if res.CommonIntegrationsObject != nil {
        // handle response
    }
}
```

### Parameters

| Parameter                                             | Type                                                  | Required                                              | Description                                           |
| ----------------------------------------------------- | ----------------------------------------------------- | ----------------------------------------------------- | ----------------------------------------------------- |
| `ctx`                                                 | [context.Context](https://pkg.go.dev/context#Context) | :heavy_check_mark:                                    | The context to use for the request.                   |


### Response

**[*operations.GetAllCommonIntegrationsResponse](../../models/operations/getallcommonintegrationsresponse.md), error**


## GetOneCommonIntegration

Get common integration

### Example Usage

```go
package main

import(
	"context"
	"log"
	"manager"
	"manager/pkg/models/operations"
)

func main() {
    s := manager.New()

    ctx := context.Background()
    res, err := s.Common.GetOneCommonIntegration(ctx, operations.GetOneCommonIntegrationRequest{
        Name: "Johnnie Stamm",
    })
    if err != nil {
        log.Fatal(err)
    }

    if res.CommonIntegrationObject != nil {
        // handle response
    }
}
```

### Parameters

| Parameter                                                                                              | Type                                                                                                   | Required                                                                                               | Description                                                                                            |
| ------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------ |
| `ctx`                                                                                                  | [context.Context](https://pkg.go.dev/context#Context)                                                  | :heavy_check_mark:                                                                                     | The context to use for the request.                                                                    |
| `request`                                                                                              | [operations.GetOneCommonIntegrationRequest](../../models/operations/getonecommonintegrationrequest.md) | :heavy_check_mark:                                                                                     | The request object to use for the request.                                                             |


### Response

**[*operations.GetOneCommonIntegrationResponse](../../models/operations/getonecommonintegrationresponse.md), error**


## PostCommonIntegration

Create common integration

### Example Usage

```go
package main

import(
	"context"
	"log"
	"manager"
	"manager/pkg/models/shared"
)

func main() {
    s := manager.New()

    ctx := context.Background()
    res, err := s.Common.PostCommonIntegration(ctx, shared.CommonIntegrationObject{
        Name: "Rick Kertzmann",
        Subscriptions: []shared.CommonIntegrationObjectSubscriptions{
            shared.CommonIntegrationObjectSubscriptions{
                Attributes: map[string]string{
                    "tempora": "suscipit",
                    "molestiae": "minus",
                    "placeat": "voluptatum",
                    "iusto": "excepturi",
                },
                Groups: []shared.CommonIntegrationObjectSubscriptionsGroups{
                    shared.CommonIntegrationObjectSubscriptionsGroups{
                        Attributes: map[string]string{
                            "temporibus": "ab",
                            "quis": "veritatis",
                            "deserunt": "perferendis",
                            "ipsam": "repellendus",
                        },
                        Name: "Cedric Connelly",
                        Values: map[string]string{
                            "molestiae": "quod",
                            "quod": "esse",
                            "totam": "porro",
                            "dolorum": "dicta",
                        },
                    },
                    shared.CommonIntegrationObjectSubscriptionsGroups{
                        Attributes: map[string]string{
                            "officia": "occaecati",
                            "fugit": "deleniti",
                            "hic": "optio",
                        },
                        Name: "Jack Johns",
                        Values: map[string]string{
                            "impedit": "cum",
                        },
                    },
                },
                Name: "Edna Mante II",
            },
        },
        Target: &shared.CommonIntegrationObjectTarget{
            Attributes: map[string]string{
                "sed": "iste",
                "dolor": "natus",
                "laboriosam": "hic",
            },
            Name: manager.String("Wilbur Kirlin"),
        },
    })
    if err != nil {
        log.Fatal(err)
    }

    if res.ResponseMessage != nil {
        // handle response
    }
}
```

### Parameters

| Parameter                                                                        | Type                                                                             | Required                                                                         | Description                                                                      |
| -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- |
| `ctx`                                                                            | [context.Context](https://pkg.go.dev/context#Context)                            | :heavy_check_mark:                                                               | The context to use for the request.                                              |
| `request`                                                                        | [shared.CommonIntegrationObject](../../models/shared/commonintegrationobject.md) | :heavy_check_mark:                                                               | The request object to use for the request.                                       |


### Response

**[*operations.PostCommonIntegrationResponse](../../models/operations/postcommonintegrationresponse.md), error**


## PutAllCommonIntegration

Update common integration

### Example Usage

```go
package main

import(
	"context"
	"log"
	"manager"
	"manager/pkg/models/operations"
	"manager/pkg/models/shared"
)

func main() {
    s := manager.New()

    ctx := context.Background()
    res, err := s.Common.PutAllCommonIntegration(ctx, operations.PutAllCommonIntegrationRequest{
        CommonIntegrationObject: shared.CommonIntegrationObject{
            Name: "Mr. Kerry Predovic",
            Subscriptions: []shared.CommonIntegrationObjectSubscriptions{
                shared.CommonIntegrationObjectSubscriptions{
                    Attributes: map[string]string{
                        "laborum": "dolores",
                        "dolorem": "corporis",
                        "explicabo": "nobis",
                    },
                    Groups: []shared.CommonIntegrationObjectSubscriptionsGroups{
                        shared.CommonIntegrationObjectSubscriptionsGroups{
                            Attributes: map[string]string{
                                "nemo": "minima",
                                "excepturi": "accusantium",
                                "iure": "culpa",
                            },
                            Name: "Darrin Brakus",
                            Values: map[string]string{
                                "consequuntur": "repellat",
                                "mollitia": "occaecati",
                                "numquam": "commodi",
                            },
                        },
                        shared.CommonIntegrationObjectSubscriptionsGroups{
                            Attributes: map[string]string{
                                "molestiae": "velit",
                                "error": "quia",
                            },
                            Name: "Gloria Padberg",
                            Values: map[string]string{
                                "quo": "sequi",
                            },
                        },
                    },
                    Name: "Vernon Ondricka Sr.",
                },
                shared.CommonIntegrationObjectSubscriptions{
                    Attributes: map[string]string{
                        "temporibus": "laborum",
                        "quasi": "reiciendis",
                        "voluptatibus": "vero",
                    },
                    Groups: []shared.CommonIntegrationObjectSubscriptionsGroups{
                        shared.CommonIntegrationObjectSubscriptionsGroups{
                            Attributes: map[string]string{
                                "voluptatibus": "ipsa",
                                "omnis": "voluptate",
                                "cum": "perferendis",
                            },
                            Name: "Bessie Grady II",
                            Values: map[string]string{
                                "iusto": "dicta",
                                "harum": "enim",
                            },
                        },
                        shared.CommonIntegrationObjectSubscriptionsGroups{
                            Attributes: map[string]string{
                                "commodi": "repudiandae",
                                "quae": "ipsum",
                                "quidem": "molestias",
                                "excepturi": "pariatur",
                            },
                            Name: "Irma Ledner DVM",
                            Values: map[string]string{
                                "veritatis": "itaque",
                                "incidunt": "enim",
                                "consequatur": "est",
                            },
                        },
                    },
                    Name: "Benjamin O'Connell",
                },
                shared.CommonIntegrationObjectSubscriptions{
                    Attributes: map[string]string{
                        "modi": "qui",
                        "aliquid": "cupiditate",
                    },
                    Groups: []shared.CommonIntegrationObjectSubscriptionsGroups{
                        shared.CommonIntegrationObjectSubscriptionsGroups{
                            Attributes: map[string]string{
                                "magni": "assumenda",
                            },
                            Name: "Linda Corkery",
                            Values: map[string]string{
                                "facilis": "tempore",
                                "labore": "delectus",
                            },
                        },
                        shared.CommonIntegrationObjectSubscriptionsGroups{
                            Attributes: map[string]string{
                                "non": "eligendi",
                                "sint": "aliquid",
                            },
                            Name: "Terence Marquardt",
                            Values: map[string]string{
                                "a": "dolorum",
                                "in": "in",
                                "illum": "maiores",
                                "rerum": "dicta",
                            },
                        },
                        shared.CommonIntegrationObjectSubscriptionsGroups{
                            Attributes: map[string]string{
                                "cumque": "facere",
                                "ea": "aliquid",
                            },
                            Name: "Tomas Friesen",
                            Values: map[string]string{
                                "delectus": "quidem",
                                "provident": "nam",
                                "id": "blanditiis",
                                "deleniti": "sapiente",
                            },
                        },
                    },
                    Name: "Sandy Huels",
                },
            },
            Target: &shared.CommonIntegrationObjectTarget{
                Attributes: map[string]string{
                    "molestiae": "perferendis",
                    "nihil": "magnam",
                    "distinctio": "id",
                },
                Name: manager.String("Jamie Hoppe"),
            },
        },
        Name: "Mrs. Meghan Collins V",
    })
    if err != nil {
        log.Fatal(err)
    }

    if res.ResponseMessage != nil {
        // handle response
    }
}
```

### Parameters

| Parameter                                                                                              | Type                                                                                                   | Required                                                                                               | Description                                                                                            |
| ------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------ |
| `ctx`                                                                                                  | [context.Context](https://pkg.go.dev/context#Context)                                                  | :heavy_check_mark:                                                                                     | The context to use for the request.                                                                    |
| `request`                                                                                              | [operations.PutAllCommonIntegrationRequest](../../models/operations/putallcommonintegrationrequest.md) | :heavy_check_mark:                                                                                     | The request object to use for the request.                                                             |


### Response

**[*operations.PutAllCommonIntegrationResponse](../../models/operations/putallcommonintegrationresponse.md), error**

