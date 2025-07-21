# \TranslateApi

All URIs are relative to *https://kagi.com/api/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**translate**](TranslateApi.md#translate) | **POST** /api/translate | Text Translation
[**translate_alternatives**](TranslateApi.md#translate_alternatives) | **POST** /alternative-translations | Alternative Translations
[**translate_detect**](TranslateApi.md#translate_detect) | **POST** /api/detect | Language Detection
[**translate_dictionary**](TranslateApi.md#translate_dictionary) | **POST** /api/dictionary | Dictionary
[**translate_list_languages**](TranslateApi.md#translate_list_languages) | **GET** /api/list-languages | List Supported Languages
[**translate_romanize**](TranslateApi.md#translate_romanize) | **GET** /api/romanize | Text Romanization
[**translate_word_insights**](TranslateApi.md#translate_word_insights) | **POST** /api/word-insights | Word Insights



## translate

> models::Translate200Response translate(translate_request)
Text Translation

Translates text between languages with customizable options for gender, formality, and style. Supports both single text translation and efficient batch translation of multiple text snippets with context awareness.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**translate_request** | [**TranslateRequest**](TranslateRequest.md) |  | [required] |

### Return type

[**models::Translate200Response**](translate_200_response.md)

### Authorization

[kagi-translate](../README.md#kagi-translate)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, text/event-stream

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## translate_alternatives

> models::TranslateAlternatives200Response translate_alternatives(original_text, existing_translation, target_lang, source_lang, target_explanation_language, translation_options, partial_translation)
Alternative Translations

Provides alternative translation options for a given text with explanations. Supports two modes: standard mode (alternatives for a full translation) and partial mode (alternative ways to phrase a specific part of a translation).

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**original_text** | **String** | Original text to translate. In partial mode, this serves as context for the phrase (may be ignored if not relevant). | [required] |
**existing_translation** | **String** | In standard mode: existing full translation of the original text. In partial mode: the specific phrase you want alternative ways to express. | [required] |
**target_lang** | **String** | Target language code (ISO-639) for the translations | [required] |
**source_lang** | Option<**String**> | Source language code (ISO-639) of the original text. Helps provide more accurate alternatives by understanding language-specific nuances. |  |
**target_explanation_language** | Option<**String**> | Language code (ISO-639) for the explanations |  |[default to en]
**translation_options** | Option<**String**> | JSON string with translation customization options: - `formality`: Controls formality level [\\\"default\\\", \\\"more\\\", \\\"less\\\"] - `speaker_gender`: Gender of the speaker [\\\"unknown\\\", \\\"feminine\\\", \\\"masculine\\\", \\\"neutral\\\"] - `addressee_gender`: Gender of the person being addressed [\\\"unknown\\\", \\\"feminine\\\", \\\"masculine\\\", \\\"neutral\\\"] - `style`: Translation style [\\\"natural\\\", \\\"literal\\\"] - `context`: Additional context to inform translation (string)  |  |
**partial_translation** | Option<**String**> | Mode switch: 'false' for standard mode (full translation alternatives), 'true' for partial mode (alternative ways to phrase a specific part) |  |[default to false]

### Return type

[**models::TranslateAlternatives200Response**](translateAlternatives_200_response.md)

### Authorization

[kagi-translate](../README.md#kagi-translate)

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## translate_detect

> models::TranslateDetect200Response translate_detect(translate_detect_request)
Language Detection

Detects the language of the provided text.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**translate_detect_request** | [**TranslateDetectRequest**](TranslateDetectRequest.md) |  | [required] |

### Return type

[**models::TranslateDetect200Response**](translateDetect_200_response.md)

### Authorization

[kagi-translate](../README.md#kagi-translate)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## translate_dictionary

> models::TranslateDictionary200Response translate_dictionary(translate_dictionary_request)
Dictionary

Provides dictionary definitions for words in different languages.  **Translation behavior:** - Fields translated to `definition_language`: definition, notes, etymology, part_of_speech, usage_level, dialect - Fields that remain in `word_language`: word, synonyms, pronunciation, plural, related_words, examples (with translations in parentheses when languages differ) - Fields always in English (strict enums): gender (\"masculine\", \"feminine\", \"neuter\", \"common\"), temporal_trend (\"increasing\", \"stable\", \"decreasing\") 

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**translate_dictionary_request** | [**TranslateDictionaryRequest**](TranslateDictionaryRequest.md) |  | [required] |

### Return type

[**models::TranslateDictionary200Response**](translateDictionary_200_response.md)

### Authorization

[kagi-translate](../README.md#kagi-translate)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, text/plain

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## translate_list_languages

> Vec<models::TranslateListLanguages200ResponseInner> translate_list_languages(r#type, locale)
List Supported Languages

Returns a list of languages supported by the translation API.  The response includes language codes, names, and whether each language supports formality settings. 

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**r#type** | Option<**String**> | Type of languages to return ('source' or 'target') |  |
**locale** | Option<**String**> | Locale code to use for language names (e.g., 'en', 'de', 'fr') |  |

### Return type

[**Vec<models::TranslateListLanguages200ResponseInner>**](translateListLanguages_200_response_inner.md)

### Authorization

[kagi-translate](../README.md#kagi-translate)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## translate_romanize

> models::TranslateRomanize200Response translate_romanize(text, language)
Text Romanization

Converts non-Latin script text to Latin script (romanization/transliteration). Uses standardized romanization styles for each language: Hepburn for Japanese, Pinyin for Chinese, ALA-LC for Arabic, etc.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**text** | **String** | Text to romanize | [required] |
**language** | **String** | Language code (ISO-639) of the source text | [required] |

### Return type

[**models::TranslateRomanize200Response**](translateRomanize_200_response.md)

### Authorization

[kagi-translate](../README.md#kagi-translate)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## translate_word_insights

> models::TranslateWordInsights200Response translate_word_insights(original_text, translated_text, target_explanation_language, translation_options)
Word Insights

Provides detailed linguistic insights and alternatives for translated text. The API identifies 3-5 key words or phrases in the translated text that have meaningful alternative expressions, and returns:  1. A marked version of the translation with insight markers 2. Alternative expressions for each identified word/phrase 3. Brief explanations for each alternative in the target explanation language 4. Type labels categorizing each insight (e.g., \"Lexical choice\", \"Cultural reference\") 

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**original_text** | **String** | Source text that was translated | [required] |
**translated_text** | **String** | Translated text to analyze for linguistic insights | [required] |
**target_explanation_language** | Option<**String**> | Language code (ISO-639) for the explanations and type labels |  |[default to en]
**translation_options** | Option<**String**> | Optional JSON string with translation options that provide context for the insights. Can include formality, gender preferences, and style.  |  |

### Return type

[**models::TranslateWordInsights200Response**](translateWordInsights_200_response.md)

### Authorization

[kagi-translate](../README.md#kagi-translate)

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

