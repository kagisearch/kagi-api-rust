# \EnrichmentApi

All URIs are relative to *https://kagi.com/api/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**enrich_search**](EnrichmentApi.md#enrich_search) | **GET** /enrich/{type} | Get enriched search results



## enrich_search

> models::EnrichSearch200Response enrich_search(q, r#type)
Get enriched search results

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**q** | **String** | Query to enrich | [required] |
**r#type** | **String** | Enrich a search query with results pulled from Kagi indexes. | [required] |[default to web]

### Return type

[**models::EnrichSearch200Response**](enrichSearch_200_response.md)

### Authorization

[kagi](../README.md#kagi)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

