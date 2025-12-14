# \CosmeticsApi

All URIs are relative to *https://api.dofusdu.de*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_all_cosmetics_list**](CosmeticsApi.md#get_all_cosmetics_list) | **GET** /{game}/v1/{language}/items/cosmetics/all | List All Cosmetics
[**get_cosmetics_list**](CosmeticsApi.md#get_cosmetics_list) | **GET** /{game}/v1/{language}/items/cosmetics | List Cosmetics
[**get_cosmetics_search**](CosmeticsApi.md#get_cosmetics_search) | **GET** /{game}/v1/{language}/items/cosmetics/search | Search Cosmetics
[**get_cosmetics_single**](CosmeticsApi.md#get_cosmetics_single) | **GET** /{game}/v1/{language}/items/cosmetics/{ankama_id} | Single Cosmetics



## get_all_cosmetics_list

> models::ListItems get_all_cosmetics_list(language, game, sort_left_square_bracket_level_right_square_bracket, filter_left_square_bracket_min_level_right_square_bracket, filter_left_square_bracket_max_level_right_square_bracket, accept_encoding, filter_left_square_bracket_type_name_id_right_square_bracket)
List All Cosmetics

Retrieve all cosmetic items with one request. This endpoint is just an alias for the a list with disabled pagination (page[size]=-1) and all fields[type] set.  If you want everything unfiltered, delete the other query parameters.  Be careful with testing or (god forbid) using /all in your browser, the returned json is huge and will slow down the browser!  Tip: set the HTTP Header 'Accept-Encoding: gzip' for saving bandwidth. You will need to uncompress it on your end. Example with cURL: ``` curl -sH 'Accept-Encoding: gzip' <api-endpoint> | gunzip - ```

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**language** | **String** | a valid language code | [required] |
**game** | **String** | game main 'dofus3' or beta channel 'dofus3beta' | [required] |
**sort_left_square_bracket_level_right_square_bracket** | Option<**String**> | sort the resulting list by level, default unsorted |  |
**filter_left_square_bracket_min_level_right_square_bracket** | Option<**i32**> | only results which level is equal or above this value |  |
**filter_left_square_bracket_max_level_right_square_bracket** | Option<**i32**> | only results which level is equal or below this value |  |
**accept_encoding** | Option<**String**> | optional compression for saving bandwidth |  |
**filter_left_square_bracket_type_name_id_right_square_bracket** | Option<[**Vec<String>**](String.md)> | multi-filter results with the english type name. Add with \"wood\" or \"+wood\" and exclude with \"-wood\". |  |

### Return type

[**models::ListItems**](ListItems.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_cosmetics_list

> models::ListItems get_cosmetics_list(language, game, sort_left_square_bracket_level_right_square_bracket, filter_left_square_bracket_min_level_right_square_bracket, filter_left_square_bracket_max_level_right_square_bracket, page_left_square_bracket_size_right_square_bracket, page_left_square_bracket_number_right_square_bracket, fields_left_square_bracket_item_right_square_bracket, filter_left_square_bracket_type_name_id_right_square_bracket)
List Cosmetics

Retrieve a list of cosmetic items.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**language** | **String** | a valid language code | [required] |
**game** | **String** | game main 'dofus3' or beta channel 'dofus3beta' | [required] |
**sort_left_square_bracket_level_right_square_bracket** | Option<**String**> | sort the resulting list by level, default unsorted |  |
**filter_left_square_bracket_min_level_right_square_bracket** | Option<**i32**> | only results which level is equal or above this value |  |
**filter_left_square_bracket_max_level_right_square_bracket** | Option<**i32**> | only results which level is equal or below this value |  |
**page_left_square_bracket_size_right_square_bracket** | Option<**i32**> | size of the results from the list. -1 disables pagination and gets all in one response. |  |
**page_left_square_bracket_number_right_square_bracket** | Option<**i32**> | page number based on the current page[size]. So you could get page 1 with 8 entrys and page 2 would have entries 8 to 16. |  |
**fields_left_square_bracket_item_right_square_bracket** | Option<[**Vec<String>**](String.md)> | adds fields from their detail endpoint to the item list entries. Multiple comma separated values allowed. |  |
**filter_left_square_bracket_type_name_id_right_square_bracket** | Option<[**Vec<String>**](String.md)> | multi-filter results with the english type name. Add with \"wood\" or \"+wood\" and exclude with \"-wood\". |  |

### Return type

[**models::ListItems**](ListItems.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_cosmetics_search

> Vec<models::ListItem> get_cosmetics_search(language, game, query, filter_left_square_bracket_min_level_right_square_bracket, filter_left_square_bracket_max_level_right_square_bracket, limit, filter_left_square_bracket_type_name_id_right_square_bracket)
Search Cosmetics

Search in all names and descriptions of cosmetic items with a query.

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

[**Vec<models::ListItem>**](ListItem.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_cosmetics_single

> models::Equipment get_cosmetics_single(language, ankama_id, game)
Single Cosmetics

Retrieve a specific cosmetic item with id.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**language** | **String** | a valid language code | [required] |
**ankama_id** | **i32** | identifier | [required] |
**game** | **String** | game main 'dofus3' or beta channel 'dofus3beta' | [required] |

### Return type

[**models::Equipment**](Equipment.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

