# \FastGptApi

All URIs are relative to *https://kagi.com/api/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**fast_gpt**](FastGptApi.md#fast_gpt) | **POST** /fastgpt | Answer a query.



## fast_gpt

> models::FastGpt200Response fast_gpt(fast_gpt_request)
Answer a query.

FastGPT is a Kagi service using powerful LLMs to answer user queries running a full search engine underneath. Think ChatGPT, but on steroids and faster! You can try the web app here.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**fast_gpt_request** | [**FastGptRequest**](FastGptRequest.md) | Contains the query to process. | [required] |

### Return type

[**models::FastGpt200Response**](fastGPT_200_response.md)

### Authorization

[kagi](../README.md#kagi)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

