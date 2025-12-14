# \MountsApi

All URIs are relative to *https://api.dofusdu.de*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_all_mounts_list**](MountsApi.md#get_all_mounts_list) | **GET** /{game}/v1/{language}/mounts/all | List All Mounts
[**get_mounts_list**](MountsApi.md#get_mounts_list) | **GET** /{game}/v1/{language}/mounts | List Mounts
[**get_mounts_search**](MountsApi.md#get_mounts_search) | **GET** /{game}/v1/{language}/mounts/search | Search Mounts
[**get_mounts_single**](MountsApi.md#get_mounts_single) | **GET** /{game}/v1/{language}/mounts/{ankama_id} | Single Mounts



## get_all_mounts_list

> models::ListMounts get_all_mounts_list(language, game, filter_left_square_bracket_family_name_right_square_bracket, accept_encoding, filter_left_square_bracket_family_id_right_square_bracket)
List All Mounts

Retrieve all mounts with one request. This endpoint is just an alias for the a list with disabled pagination (page[size]=-1) and all fields[type] set.  If you want everything unfiltered, delete the other query parameters.  Be careful with testing or (god forbid) using /all in your browser, the returned json is huge and will slow down the browser!  Tip: set the HTTP Header 'Accept-Encoding: gzip' for saving bandwidth. You will need to uncompress it on your end. Example with cURL: ``` curl -sH 'Accept-Encoding: gzip' <api-endpoint> | gunzip - ```

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**language** | **String** | a valid language code | [required] |
**game** | **String** | game main 'dofus3' or beta channel 'dofus3beta' | [required] |
**filter_left_square_bracket_family_name_right_square_bracket** | Option<**String**> | only results with the translated family name |  |
**accept_encoding** | Option<**String**> | optional compression for saving bandwidth |  |
**filter_left_square_bracket_family_id_right_square_bracket** | Option<**i32**> | only results with the unique family id |  |

### Return type

[**models::ListMounts**](ListMounts.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_mounts_list

> models::ListMounts get_mounts_list(language, game, filter_left_square_bracket_family_name_right_square_bracket, page_left_square_bracket_size_right_square_bracket, page_left_square_bracket_number_right_square_bracket, fields_left_square_bracket_mount_right_square_bracket, filter_left_square_bracket_family_id_right_square_bracket)
List Mounts

Retrieve a list of mounts.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**language** | **String** | a valid language code | [required] |
**game** | **String** | game main 'dofus3' or beta channel 'dofus3beta' | [required] |
**filter_left_square_bracket_family_name_right_square_bracket** | Option<**String**> | only results with the translated family name |  |
**page_left_square_bracket_size_right_square_bracket** | Option<**i32**> | size of the results from the list. -1 disables pagination and gets all in one response. |  |
**page_left_square_bracket_number_right_square_bracket** | Option<**i32**> | page number based on the current page[size]. So you could get page 1 with 8 entrys and page 2 would have entries 8 to 16. |  |
**fields_left_square_bracket_mount_right_square_bracket** | Option<[**Vec<String>**](String.md)> | adds fields from their detail endpoint to the item list entries. Multiple comma separated values allowed. |  |
**filter_left_square_bracket_family_id_right_square_bracket** | Option<**i32**> | only results with the unique family id |  |

### Return type

[**models::ListMounts**](ListMounts.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_mounts_search

> Vec<models::Mount> get_mounts_search(language, game, query, filter_left_square_bracket_family_name_right_square_bracket, limit, filter_left_square_bracket_family_id_right_square_bracket)
Search Mounts

Search in all names and descriptions of mounts with a query.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**language** | **String** | a valid language code | [required] |
**game** | **String** | game main 'dofus3' or beta channel 'dofus3beta' | [required] |
**query** | **String** | case sensitive search query | [required] |
**filter_left_square_bracket_family_name_right_square_bracket** | Option<**String**> | only results with the translated family name |  |
**limit** | Option<**i32**> | maximum number of returned results |  |[default to 8]
**filter_left_square_bracket_family_id_right_square_bracket** | Option<**i32**> | only results with the unique family id |  |

### Return type

[**Vec<models::Mount>**](Mount.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_mounts_single

> models::Mount get_mounts_single(language, ankama_id, game)
Single Mounts

Retrieve a specific mount with id.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**language** | **String** | a valid language code | [required] |
**ankama_id** | **i32** | identifier | [required] |
**game** | **String** | game main 'dofus3' or beta channel 'dofus3beta' | [required] |

### Return type

[**models::Mount**](Mount.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

