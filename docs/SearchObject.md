# SearchObject

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**t** | Option<**i32**> | This is always set to 0. It is used as a flag to identify if the result was a rearch result or a related searches object. | [optional]
**rank** | Option<**i32**> | Order of resarch results, the highest rank is 1 and should identify results that match the search request better. | [optional]
**url** | Option<**String**> | URL of the resource identified in the search result. | [optional]
**title** | Option<**String**> | Title of the search result. This can be taken from the title of the html document, or the title of a media resource. | [optional]
**snippet** | Option<**String**> | a short desciption, or summary, of the content. | [optional]
**published** | Option<**String**> | the date the rearch result was created | [optional]
**thumbnail** | Option<[**models::SearchObjectThumbnail**](searchObject_thumbnail.md)> |  | [optional]
**image** | Option<[**models::SearchObjectImage**](searchObject_image.md)> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


