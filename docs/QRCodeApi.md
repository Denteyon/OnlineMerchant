# OnlineMerchant.QRCodeApi

All URIs are relative to *http://localhost:1337*

Method | HTTP request | Description
------------- | ------------- | -------------
[**thirdpartyMerchantRequestQRPaymentPost**](QRCodeApi.md#thirdpartyMerchantRequestQRPaymentPost) | **POST** /thirdparty/merchant/requestQRPayment | Get payment code



## thirdpartyMerchantRequestQRPaymentPost

> InlineResponse2001 thirdpartyMerchantRequestQRPaymentPost(authorization, body)

Get payment code

### Example

```javascript
import OnlineMerchant from 'online_merchant';
let defaultClient = OnlineMerchant.ApiClient.instance;
// Configure OAuth2 access token for authorization: default
let default = defaultClient.authentications['default'];
default.accessToken = 'YOUR ACCESS TOKEN';

let apiInstance = new OnlineMerchant.QRCodeApi();
let authorization = "'Bearer {user_token}'"; // String | 
let body = new OnlineMerchant.InlineObject1(); // InlineObject1 | 
apiInstance.thirdpartyMerchantRequestQRPaymentPost(authorization, body, (error, data, response) => {
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
 **authorization** | **String**|  | [default to &#39;Bearer {user_token}&#39;]
 **body** | [**InlineObject1**](InlineObject1.md)|  | 

### Return type

[**InlineResponse2001**](InlineResponse2001.md)

### Authorization

[default](../README.md#default)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: */*

