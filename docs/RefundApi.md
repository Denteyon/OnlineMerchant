# OnlineMerchant.RefundApi

All URIs are relative to *http://localhost:1337*

Method | HTTP request | Description
------------- | ------------- | -------------
[**thirdpartyMerchantRefundPaymentPost**](RefundApi.md#thirdpartyMerchantRefundPaymentPost) | **POST** /thirdparty/merchant/refundPayment | Refund for a Payment



## thirdpartyMerchantRefundPaymentPost

> InlineResponse2002 thirdpartyMerchantRefundPaymentPost(authorization, body)

Refund for a Payment

### Example

```javascript
import OnlineMerchant from 'online_merchant';
let defaultClient = OnlineMerchant.ApiClient.instance;
// Configure OAuth2 access token for authorization: default
let default = defaultClient.authentications['default'];
default.accessToken = 'YOUR ACCESS TOKEN';

let apiInstance = new OnlineMerchant.RefundApi();
let authorization = "'Bearer {user_token}'"; // String | 
let body = new OnlineMerchant.InlineObject3(); // InlineObject3 | 
apiInstance.thirdpartyMerchantRefundPaymentPost(authorization, body, (error, data, response) => {
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
 **body** | [**InlineObject3**](InlineObject3.md)|  | 

### Return type

[**InlineResponse2002**](InlineResponse2002.md)

### Authorization

[default](../README.md#default)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: */*

