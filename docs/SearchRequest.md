# SearchRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**query** | **String** | The search query to perform. | 
**workflow** | Option<**String**> | Can be used to filter result output to a single category. | [optional][default to Search]
**lens_id** | Option<**String**> | A lens ID, as shown on https://kagi.com/settings/lenses when a lens is set to be shareable. Can be just the ID portion of the URL (`https://kagi.com/lenses/ID`), or the full URL. | [optional]
**lens** | Option<[**models::SearchRequestLens**](search_request_lens.md)> |  | [optional]
**timeout** | Option<**f64**> | Number of seconds to allow for collecting search results. Lower values will return results more quickly, but may be lower quality or inconsistent between calls. If omitted, will use the latest recommended value by Kagi. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


