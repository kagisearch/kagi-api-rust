# SearchResult

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**url** | **String** | The location of the result. This is the direct URL to the resource that matches the query | 
**title** | **String** | This is the title of the resource. For HTML resources, it is the title in the header of the document. For Video resources, it is the name of the video that would be displayed on the video site | 
**snippet** | Option<**String**> | A short summary of the contents of the resource | [optional]
**time** | Option<**String**> | A date for when the resource was last updated or created. | [optional]
**image** | Option<[**models::SearchResultImage**](searchResult_image.md)> |  | [optional]
**props** | Option<[**std::collections::HashMap<String, serde_json::Value>**](serde_json::Value.md)> | Holds arbitrary result metadata | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


