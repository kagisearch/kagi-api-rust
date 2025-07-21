# TranslateDictionaryRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**word** | **String** | The word to look up | 
**word_language** | Option<**String**> | Language code (ISO-639) of the word, or \"auto\" for automatic detection | [optional][default to en]
**definition_language** | Option<**String**> | Language code (ISO-639) for the definition output | [optional][default to en]
**stream** | Option<**bool**> | Whether to return a streaming response with fields sent as they become available | [optional][default to false]
**nsfw** | Option<**bool**> | Whether to allow NSFW/inappropriate content. If false, returns empty definition for inappropriate words | [optional][default to true]
**model** | Option<**String**> | Optional model identifier. Can be either a model name (e.g., \"gpt-4o\", \"claude-35-sonnet\", \"gemini-flash-2.0\") or a model constant (e.g., \"ANTHROPIC_CLAUDE_35_SONNET\", \"OPENAI_GPT4O\"). See model-selection.ts for full list. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


