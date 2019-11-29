# YlThirdPartyPrequalificationApiClient.RequestsApi

All URIs are relative to *https://dev.youlendapi.com/prequalification*

Method | HTTP request | Description
------------- | ------------- | -------------
[**requestsPost**](RequestsApi.md#requestsPost) | **POST** /Requests | Initiates a prequalification of a merchant for a loan. It will use as much data as it can to do the analysis  so the more data provided the more accurate the result



## requestsPost

> PreQualificationResultDocument requestsPost(opts)

Initiates a prequalification of a merchant for a loan. It will use as much data as it can to do the analysis  so the more data provided the more accurate the result

Can add sample as an example here

### Example

```javascript
import YlThirdPartyPrequalificationApiClient from 'yl-third-party-prequalification-api-client';
let defaultClient = YlThirdPartyPrequalificationApiClient.ApiClient.instance;
// Configure OAuth2 access token for authorization: oauth2
let oauth2 = defaultClient.authentications['oauth2'];
oauth2.accessToken = 'YOUR ACCESS TOKEN';

let apiInstance = new YlThirdPartyPrequalificationApiClient.RequestsApi();
let opts = {
  'apiVersion': "apiVersion_example", // String | 
  'preQualificationModel': new YlThirdPartyPrequalificationApiClient.PreQualificationModel() // PreQualificationModel | 
};
apiInstance.requestsPost(opts).then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **apiVersion** | **String**|  | [optional] 
 **preQualificationModel** | [**PreQualificationModel**](PreQualificationModel.md)|  | [optional] 

### Return type

[**PreQualificationResultDocument**](PreQualificationResultDocument.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, application/xml

