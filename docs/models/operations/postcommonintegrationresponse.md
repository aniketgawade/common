# PostCommonIntegrationResponse


## Fields

| Field                                                             | Type                                                              | Required                                                          | Description                                                       |
| ----------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- |
| `ContentType`                                                     | *string*                                                          | :heavy_check_mark:                                                | N/A                                                               |
| `StatusCode`                                                      | *int*                                                             | :heavy_check_mark:                                                | N/A                                                               |
| `RawResponse`                                                     | [*http.Response](https://pkg.go.dev/net/http#Response)            | :heavy_minus_sign:                                                | N/A                                                               |
| `ResponseMessage`                                                 | [*shared.ResponseMessage](../../models/shared/responsemessage.md) | :heavy_minus_sign:                                                | Common integration success response                               |