# \GameApi

All URIs are relative to *https://api.dofusdu.de*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_game_search**](GameApi.md#get_game_search) | **GET** /{game}/v1/{language}/search | Game Search
[**get_items_all_search**](GameApi.md#get_items_all_search) | **GET** /{game}/v1/{language}/items/search | Search All Items



## get_game_search

> Vec<models::GameSearch> get_game_search(language, game, query, filter_left_square_bracket_search_index_right_square_bracket, limit, fields_left_square_bracket_item_right_square_bracket, filter_left_square_bracket_type_name_id_right_square_bracket)
Game Search

Search in all names and descriptions of all supported types in the game. For the list of supported types see the endpoint /dofus3/meta/search/types.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**language** | **String** | a valid language code | [required] |
**game** | **String** | game main 'dofus3' or beta channel 'dofus3beta' | [required] |
**query** | **String** | search query | [required] |
**filter_left_square_bracket_search_index_right_square_bracket** | Option<[**Vec<String>**](String.md)> | only results with all specific type |  |
**limit** | Option<**i32**> | maximum number of returned results |  |[default to 8]
**fields_left_square_bracket_item_right_square_bracket** | Option<[**Vec<String>**](String.md)> | adds fields from the item search to the list entries if the hit is an item. Multiple comma separated values allowed. |  |
**filter_left_square_bracket_type_name_id_right_square_bracket** | Option<[**Vec<String>**](String.md)> | multi-filter results with the english item type name, including \"mount\" and \"set\" from filter[search_index]. Add with \"wood\" or \"+wood\" and exclude with \"-wood\". |  |

### Return type

[**Vec<models::GameSearch>**](GameSearch.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_items_all_search

> Vec<models::ListItemGeneral> get_items_all_search(language, game, query, filter_left_square_bracket_min_level_right_square_bracket, filter_left_square_bracket_max_level_right_square_bracket, limit, filter_left_square_bracket_type_name_id_right_square_bracket)
Search All Items

Search in all names and descriptions of Dofus items (including all subtypes) with a query.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**language** | **String** | a valid language code | [required] |
**game** | **String** | game main 'dofus3' or beta channel 'dofus3beta' | [required] |
**query** | **String** | case sensitive search query | [required] |
**filter_left_square_bracket_min_level_right_square_bracket** | Option<**i32**> | only results which level is equal or above this value |  |
**filter_left_square_bracket_max_level_right_square_bracket** | Option<**i32**> | only results which level is equal or below this value |  |
**limit** | Option<**i32**> | maximum number of returned results |  |[default to 8]
**filter_left_square_bracket_type_name_id_right_square_bracket** | Option<[**Vec<String>**](String.md)> | multi-filter results with the english type name. Add with \"wood\" or \"+wood\" and exclude with \"-wood\". |  |

### Return type

[**Vec<models::ListItemGeneral>**](ListItemGeneral.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

