# OnlineMerchant.LoginApi

All URIs are relative to *http://localhost:1337*

Method | HTTP request | Description
------------- | ------------- | -------------
[**thirdpartyMerchantLoginPost**](LoginApi.md#thirdpartyMerchantLoginPost) | **POST** /thirdparty/merchant/login | Login



## thirdpartyMerchantLoginPost

> InlineResponse200 thirdpartyMerchantLoginPost(body)

Login

### Example

```javascript
import OnlineMerchant from 'online_merchant';
let defaultClient = OnlineMerchant.ApiClient.instance;
// Configure OAuth2 access token for authorization: default
let default = defaultClient.authentications['default'];
default.accessToken = 'YOUR ACCESS TOKEN';

let apiInstance = new OnlineMerchant.LoginApi();
let body = new OnlineMerchant.InlineObject(); // InlineObject | 
apiInstance.thirdpartyMerchantLoginPost(body, (error, data, response) => {
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
 **body** | [**InlineObject**](InlineObject.md)|  | 

### Return type

[**InlineResponse200**](InlineResponse200.md)

### Authorization

[default](../README.md#default)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: */*

