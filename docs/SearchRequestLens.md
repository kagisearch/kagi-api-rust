# SearchRequestLens

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**sites_included** | Option<**Vec<String>**> | A list of domains to restrict the search to. | [optional]
**sites_excluded** | Option<**Vec<String>**> | A list of domains to restrict the search to. | [optional]
**keywords_included** | Option<**Vec<String>**> | A list of keywords to filter results on, such that every result *must* contain these terms. | [optional]
**keywords_excluded** | Option<**Vec<String>**> | A list of keywords to filter results on, such that any result containing these terms is removed. | [optional]
**file_type** | Option<**String**> | A specific file type to search for. (e.g., `pdf`) | [optional]
**time_after** | Option<**String**> | Filters for web pages that have been updated or published *after* the given date (`YYYY-MM-DD`). | [optional]
**time_before** | Option<**String**> | Filters for web pages that have been updated or published *before* the given date (`YYYY-MM-DD`). | [optional]
**time_relative** | Option<**String**> | Filters for web pages that have been updated or published in the given interval, relative to today's date. | [optional]
**search_region** | Option<**String**> | Requests results localized to a specific region. Can be any valid [ISO-3166-1 Alpha-2 country code](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2#Officially_assigned_code_elements), or the special value `no_region`, that will try to get the most general results possible. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


