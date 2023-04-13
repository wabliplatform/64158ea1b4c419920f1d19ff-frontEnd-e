# TempApi.PsApi

All URIs are relative to *http://localhost:8090/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createps**](PsApi.md#createps) | **POST** /ps | Creates the data
[**deleteps**](PsApi.md#deleteps) | **DELETE** /ps/{psId} | Delete the element
[**getAllps**](PsApi.md#getAllps) | **GET** /ps/getAll | Get all the data
[**getps**](PsApi.md#getps) | **GET** /ps/{psId} | Get the element
[**updateps**](PsApi.md#updateps) | **PUT** /ps/{psId} | Updates the element



## createps

> Ps createps(ps)

Creates the data

### Example

```javascript
import TempApi from 'temp_api';

let apiInstance = new TempApi.PsApi();
let ps = new TempApi.Ps(); // Ps | data to be created
apiInstance.createps(ps, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ps** | [**Ps**](Ps.md)| data to be created | 

### Return type

[**Ps**](Ps.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteps

> deleteps(psId)

Delete the element

### Example

```javascript
import TempApi from 'temp_api';

let apiInstance = new TempApi.PsApi();
let psId = "psId_example"; // String | the Id parameter
apiInstance.deleteps(psId, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully.');
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **psId** | **String**| the Id parameter | 

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## getAllps

> [Ps] getAllps()

Get all the data

### Example

```javascript
import TempApi from 'temp_api';

let apiInstance = new TempApi.PsApi();
apiInstance.getAllps((error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**[Ps]**](Ps.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getps

> Ps getps(psId)

Get the element

### Example

```javascript
import TempApi from 'temp_api';

let apiInstance = new TempApi.PsApi();
let psId = "psId_example"; // String | the Id parameter
apiInstance.getps(psId, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **psId** | **String**| the Id parameter | 

### Return type

[**Ps**](Ps.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateps

> Ps updateps(psId, opts)

Updates the element

### Example

```javascript
import TempApi from 'temp_api';

let apiInstance = new TempApi.PsApi();
let psId = "psId_example"; // String | the Id parameter
let opts = {
  'ps': new TempApi.Ps() // Ps | data to be updated
};
apiInstance.updateps(psId, opts, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **psId** | **String**| the Id parameter | 
 **ps** | [**Ps**](Ps.md)| data to be updated | [optional] 

### Return type

[**Ps**](Ps.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

