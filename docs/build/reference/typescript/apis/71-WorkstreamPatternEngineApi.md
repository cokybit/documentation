---
title: WorkstreamPatternEngine API | TypeScript SDK
---

# WorkstreamPatternEngine API

All URIs are relative to `http://localhost:1000`

Method | HTTP request | Description
------------- | ------------- | -------------
[**workstreamPatternEngineProcessorsVisionActivate**](WorkstreamPatternEngineApi#workstreampatternengineprocessorsvisionactivate) | **POST** /workstream_pattern_engine/processors/vision/activate | /workstream_pattern_engine/processors/vision/activate [POST]
[**workstreamPatternEngineProcessorsVisionDataClear**](WorkstreamPatternEngineApi#workstreampatternengineprocessorsvisiondataclear) | **POST** /workstream_pattern_engine/processors/vision/data/clear | /workstream_pattern_engine/processors/vision/data/clear [POST]
[**workstreamPatternEngineProcessorsVisionDeactivate**](WorkstreamPatternEngineApi#workstreampatternengineprocessorsvisiondeactivate) | **POST** /workstream_pattern_engine/processors/vision/deactivate | /workstream_pattern_engine/processors/vision/deactivate [POST]
[**workstreamPatternEngineProcessorsVisionStatus**](WorkstreamPatternEngineApi#workstreampatternengineprocessorsvisionstatus) | **GET** /workstream_pattern_engine/processors/vision/status | /workstream_pattern_engine/processors/vision/status [GET]


## **workstreamPatternEngineProcessorsVisionActivate** {#workstreampatternengineprocessorsvisionactivate}
> WorkstreamPatternEngineStatus workstreamPatternEngineProcessorsVisionActivate()

This will activate your Long-Term Memory Engine. This is used to aggregate information on your user\'s desktop, specifically recording the application in focus and aggregating relevant context that will then be used to ground the copilot conversations, as well as the feed.  Note: required to be a beta user to use this feature until this is live(roughly mid to late April)

### Example {#workstreampatternengineprocessorsvisionactivate-example}

```typescript
import * as Pieces from '@pieces.app/pieces-os-client'

const configuration = Pieces.Configuration()
const apiInstance = new Pieces.WorkstreamPatternEngineApi(configuration)

const body: Pieces.WorkstreamPatternEngineProcessorsVisionActivateRequest = {
// WorkstreamPatternEngineStatus (optional)
workstreamPatternEngineStatus: ,
};

apiInstance.workstreamPatternEngineProcessorsVisionActivate(body).then((data: WorkstreamPatternEngineStatus) => {
console.log('API called successfully. Returned data: ' + data)
}).catch((error: unknown) => console.error(error))
```

### Parameters {#workstreampatternengineprocessorsvisionactivate-parameters}


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workstreamPatternEngineStatus** | **WorkstreamPatternEngineStatus**|  |


### Return type {#workstreampatternengineprocessorsvisionactivate-return-type}

[**WorkstreamPatternEngineStatus**](../models/WorkstreamPatternEngineStatus)

### HTTP request headers {#workstreampatternengineprocessorsvisionactivate-http-request-headers}

- **Content-Type**: application/json
- **Accept**: application/json, text/plain


### HTTP response details {#workstreampatternengineprocessorsvisionactivate-http-response-details}
| Status code | Description | Response headers
|-------------|-------------|------------------
**200** | OK |  -  |
**403** | Forbidden, this is not available for non-beta used until mid to late April. |  -  |
**500** | Internal Server Error |  -  |

## **workstreamPatternEngineProcessorsVisionDataClear** {#workstreampatternengineprocessorsvisiondataclear}
> workstreamPatternEngineProcessorsVisionDataClear()

This will clear the data for the Long-Term Memory Engine, specifically for our vision data.  This boy will accept ranges of time that the user wants to remove the processing from.

### Example {#workstreampatternengineprocessorsvisiondataclear-example}

```typescript
import * as Pieces from '@pieces.app/pieces-os-client'

const configuration = Pieces.Configuration()
const apiInstance = new Pieces.WorkstreamPatternEngineApi(configuration)

const body: Pieces.WorkstreamPatternEngineProcessorsVisionDataClearRequest = {
// WorkstreamPatternEngineDataCleanupRequest (optional)
workstreamPatternEngineDataCleanupRequest: ,
};

apiInstance.workstreamPatternEngineProcessorsVisionDataClear(body).then((data: void (empty response body)) => {
console.log('API called successfully. Returned data: ' + data)
}).catch((error: unknown) => console.error(error))
```

### Parameters {#workstreampatternengineprocessorsvisiondataclear-parameters}


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workstreamPatternEngineDataCleanupRequest** | **WorkstreamPatternEngineDataCleanupRequest**|  |


### Return type {#workstreampatternengineprocessorsvisiondataclear-return-type}

void (empty response body)

### HTTP request headers {#workstreampatternengineprocessorsvisiondataclear-http-request-headers}

- **Content-Type**: application/json
- **Accept**: text/plain


### HTTP response details {#workstreampatternengineprocessorsvisiondataclear-http-response-details}
| Status code | Description | Response headers
|-------------|-------------|------------------
**204** | No Content |  -  |
**403** | Forbidden, this is not available for non-beta used until mid to late April. |  -  |
**500** | Internal Server Error |  -  |

## **workstreamPatternEngineProcessorsVisionDeactivate** {#workstreampatternengineprocessorsvisiondeactivate}
> WorkstreamPatternEngineStatus workstreamPatternEngineProcessorsVisionDeactivate()

This will deactivate your Long-Term Memory Engine. This is used to aggregate information on your user\'s desktop, specifically recording the application in focus and aggregating relevant context that will then be used to ground the copilot conversations, as well as the feed.  Note: required to be a beta user to use this feature until this is live(roughly mid to late April)

### Example {#workstreampatternengineprocessorsvisiondeactivate-example}

```typescript
import * as Pieces from '@pieces.app/pieces-os-client'

const configuration = Pieces.Configuration()
const apiInstance = new Pieces.WorkstreamPatternEngineApi(configuration)

const body: Pieces.WorkstreamPatternEngineProcessorsVisionDeactivateRequest = {
// WorkstreamPatternEngineStatus (optional)
workstreamPatternEngineStatus: ,
};

apiInstance.workstreamPatternEngineProcessorsVisionDeactivate(body).then((data: WorkstreamPatternEngineStatus) => {
console.log('API called successfully. Returned data: ' + data)
}).catch((error: unknown) => console.error(error))
```

### Parameters {#workstreampatternengineprocessorsvisiondeactivate-parameters}


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workstreamPatternEngineStatus** | **WorkstreamPatternEngineStatus**|  |


### Return type {#workstreampatternengineprocessorsvisiondeactivate-return-type}

[**WorkstreamPatternEngineStatus**](../models/WorkstreamPatternEngineStatus)

### HTTP request headers {#workstreampatternengineprocessorsvisiondeactivate-http-request-headers}

- **Content-Type**: application/json
- **Accept**: application/json, text/plain


### HTTP response details {#workstreampatternengineprocessorsvisiondeactivate-http-response-details}
| Status code | Description | Response headers
|-------------|-------------|------------------
**200** | OK |  -  |
**403** | Forbidden, this is not available for non-beta used until mid to late April. |  -  |
**500** | Internal Server Error |  -  |

## **workstreamPatternEngineProcessorsVisionStatus** {#workstreampatternengineprocessorsvisionstatus}
> WorkstreamPatternEngineStatus workstreamPatternEngineProcessorsVisionStatus()

This will get a snapshot of the status your Long-Term Memory Engine. This is used to aggregate information on your user\'s desktop, specifically recording the application in focus and aggregating relevant context that will then be used to ground the copilot conversations, as well as the feed.  Note: required to be a beta user to use this feature until this is live(roughly mid to late April)

### Example {#workstreampatternengineprocessorsvisionstatus-example}

```typescript
import * as Pieces from '@pieces.app/pieces-os-client'

const configuration = Pieces.Configuration()
const apiInstance = new Pieces.WorkstreamPatternEngineApi(configuration)

apiInstance.workstreamPatternEngineProcessorsVisionStatus().then((data: WorkstreamPatternEngineStatus) => {
console.log('API called successfully. Returned data: ' + data)
}).catch((error: unknown) => console.error(error))
```

### Parameters {#workstreampatternengineprocessorsvisionstatus-parameters}

This endpoint does not need any parameters.


### Return type {#workstreampatternengineprocessorsvisionstatus-return-type}

[**WorkstreamPatternEngineStatus**](../models/WorkstreamPatternEngineStatus)

### HTTP request headers {#workstreampatternengineprocessorsvisionstatus-http-request-headers}

- **Content-Type**: Not defined
- **Accept**: application/json, text/plain


### HTTP response details {#workstreampatternengineprocessorsvisionstatus-http-response-details}
| Status code | Description | Response headers
|-------------|-------------|------------------
**200** | OK |  -  |
**403** | Forbidden, this is not available for non-beta used until mid to late April. |  -  |
**500** | Internal Server Error |  -  |


