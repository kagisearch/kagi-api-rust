# Search200ResponseData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**search** | Option<[**Vec<models::SearchResult>**](searchResult.md)> | Contains all search results for html pages or wedbsites. | [optional]
**image** | Option<[**Vec<models::SearchResult>**](searchResult.md)> | Contains all search results for images. | [optional]
**video** | Option<[**Vec<models::SearchResult>**](searchResult.md)> | Contains all search results for videos. | [optional]
**podcast** | Option<[**Vec<models::SearchResult>**](searchResult.md)> | Contains all search results for podcasts. | [optional]
**podcast_creator** | Option<[**Vec<models::SearchResult>**](searchResult.md)> | Contains all search results for creators of podcasta. | [optional]
**news** | Option<[**Vec<models::SearchResult>**](searchResult.md)> | Contains all search results for news articles. | [optional]
**adjacent_question** | Option<[**Vec<models::SearchResult>**](searchResult.md)> | Contains results that are obtained by searching for slightly different queries. These questions are stored under the `props.question` path. | [optional]
**direct_answer** | Option<[**Vec<models::SearchResult>**](searchResult.md)> | If the search query was a math equation, or unit conversions, things that can be answered quickly, the result will be in here. | [optional]
**interesting_news** | Option<[**Vec<models::SearchResult>**](searchResult.md)> | Contains news results from publishers collected and stored in Kagis' news index. | [optional]
**interesting_finds** | Option<[**Vec<models::SearchResult>**](searchResult.md)> | Contains small web results from publishers collected and stored in Kagis' small web index. | [optional]
**infobox** | Option<[**Vec<models::SearchResult>**](searchResult.md)> | Contains detailed summary and tabulated information about a person, place, or thing. | [optional]
**code** | Option<[**Vec<models::SearchResult>**](searchResult.md)> | Contains all search results that link to code resources or repositories. | [optional]
**package_tracking** | Option<[**Vec<models::SearchResult>**](searchResult.md)> | If the search query was a package tracking number, the correct package tracking website should be present in this collection. | [optional]
**public_records** | Option<[**Vec<models::SearchResult>**](searchResult.md)> | Contains all search results for public records, such as government documents, or public court records. | [optional]
**weather** | Option<[**Vec<models::SearchResult>**](searchResult.md)> | Contains all search results for the current weather. | [optional]
**related_search** | Option<[**Vec<models::SearchResult>**](searchResult.md)> | Contains a list of searches that are related to the current search, and may help narrow down the results. | [optional]
**listicle** | Option<[**Vec<models::SearchResult>**](searchResult.md)> | Contains all search results that are lists of things. Results with titles like \"5 things you didn't know about...\", or \"10 of the best headphones\". | [optional]
**web_archive** | Option<[**Vec<models::SearchResult>**](searchResult.md)> | Contains all search results for archived websites that may not be available anymore | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


