# \SummarizerApi

All URIs are relative to *https://kagi.com/api/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**summarize_text**](SummarizerApi.md#summarize_text) | **POST** /summarize | Upload text to summarize.
[**summarize_url**](SummarizerApi.md#summarize_url) | **GET** /summarize | Get a summary for a URL



## summarize_text

> models::Summary summarize_text(upload_text, engine, summary_type, target_language, cache)
Upload text to summarize.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**upload_text** | [**UploadText**](UploadText.md) | Text to summarize | [required] |
**engine** | Option<**String**> | Different summarization engines are provided that will give you choices over the \"flavor\" of the summarization text. |  |[default to cecil]
**summary_type** | Option<**String**> | Different summary types are provided that control the structure of the summary output. |  |[default to summary]
**target_language** | Option<**String**> | The summarizer can translate the output into a desired language, using the table of supported language codes below.  If no language is specified, the document's original language is allowed to influence the summarizer's output. Specifying a language will add an explicit translation step, to translate the summary to the desired language.  For example, if a document is mostly written in Spanish, the summary output may itself be in Spanish or contain Spanish passages. Specifying \"EN\" will ensure all passages are translated as English.  |  |
**cache** | Option<**bool**> | Whether to allow cached requests & responses. |  |[default to true]

### Return type

[**models::Summary**](summary.md)

### Authorization

[kagi](../README.md#kagi)

### HTTP request headers

- **Content-Type**: application/json, x-www-form-urlencoded
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## summarize_url

> models::Summary summarize_url(url, engine, summary_type, target_language, cache)
Get a summary for a URL

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**url** | **String** | A URL to a document to summarize. | [required] |
**engine** | Option<**String**> | Different summarization engines are provided that will give you choices over the \"flavor\" of the summarization text. |  |[default to cecil]
**summary_type** | Option<**String**> | Different summary types are provided that control the structure of the summary output. |  |[default to summary]
**target_language** | Option<**String**> | The summarizer can translate the output into a desired language, using the table of supported language codes below.  If no language is specified, the document's original language is allowed to influence the summarizer's output. Specifying a language will add an explicit translation step, to translate the summary to the desired language.  For example, if a document is mostly written in Spanish, the summary output may itself be in Spanish or contain Spanish passages. Specifying \"EN\" will ensure all passages are translated as English.  |  |
**cache** | Option<**bool**> | Whether to allow cached requests & responses. |  |[default to true]

### Return type

[**models::Summary**](summary.md)

### Authorization

[kagi](../README.md#kagi)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

