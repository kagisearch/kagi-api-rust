# \SearchApi

All URIs are relative to *https://kagi.com/api/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**search**](SearchApi.md#search) | **POST** /search | Perform a search of the web.



## search

> models::Search200Response search(search_request)
Perform a search of the web.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**search_request** | [**SearchRequest**](SearchRequest.md) | Contains the search query to run | [required] |

### Return type

[**models::Search200Response**](search_200_response.md)

### Authorization

[kagi](../README.md#kagi)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

