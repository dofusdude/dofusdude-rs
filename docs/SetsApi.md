# \SetsApi

All URIs are relative to *https://api.dofusdu.de*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_all_sets_list**](SetsApi.md#get_all_sets_list) | **GET** /{game}/v1/{language}/sets/all | List All Sets
[**get_sets_list**](SetsApi.md#get_sets_list) | **GET** /{game}/v1/{language}/sets | List Sets
[**get_sets_search**](SetsApi.md#get_sets_search) | **GET** /{game}/v1/{language}/sets/search | Search Sets
[**get_sets_single**](SetsApi.md#get_sets_single) | **GET** /{game}/v1/{language}/sets/{ankama_id} | Single Sets



## get_all_sets_list

> models::ListEquipmentSets get_all_sets_list(language, game, sort_left_square_bracket_level_right_square_bracket, filter_left_square_bracket_min_highest_equipment_level_right_square_bracket, filter_left_square_bracket_max_highest_equipment_level_right_square_bracket, accept_encoding, filter_left_square_bracket_contains_cosmetics_only_right_square_bracket, filter_left_square_bracket_contains_cosmetics_right_square_bracket)
List All Sets

Retrieve all sets with one request. This endpoint is just an alias for the a list with disabled pagination (page[size]=-1) and all fields[type] set.  If you want everything unfiltered, delete the other query parameters.  Be careful with testing or (god forbid) using /all in your browser, the returned json is huge and will slow down the browser!  Tip: set the HTTP Header 'Accept-Encoding: gzip' for saving bandwidth. You will need to uncompress it on your end. Example with cURL: ``` curl -sH 'Accept-Encoding: gzip' <api-endpoint> | gunzip - ```

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**language** | **String** | a valid language code | [required] |
**game** | **String** | game main 'dofus3' or beta channel 'dofus3beta' | [required] |
**sort_left_square_bracket_level_right_square_bracket** | Option<**String**> | sort the resulting list by level, default unsorted |  |
**filter_left_square_bracket_min_highest_equipment_level_right_square_bracket** | Option<**i32**> | only results where the equipment with the highest level is above or equal to this value |  |
**filter_left_square_bracket_max_highest_equipment_level_right_square_bracket** | Option<**i32**> | only results where the equipment with the highest level is below or equal to this value |  |
**accept_encoding** | Option<**String**> | optional compression for saving bandwidth |  |
**filter_left_square_bracket_contains_cosmetics_only_right_square_bracket** | Option<**bool**> | filter sets based on if they only got cosmetic items in it. If true, the item ids are for the cosmetic endpoints instead of equipment. |  |
**filter_left_square_bracket_contains_cosmetics_right_square_bracket** | Option<**bool**> | filter sets based on if they got cosmetic items in it. |  |

### Return type

[**models::ListEquipmentSets**](ListEquipmentSets.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_sets_list

> models::ListEquipmentSets get_sets_list(language, game, sort_left_square_bracket_level_right_square_bracket, filter_left_square_bracket_min_highest_equipment_level_right_square_bracket, filter_left_square_bracket_max_highest_equipment_level_right_square_bracket, page_left_square_bracket_size_right_square_bracket, page_left_square_bracket_number_right_square_bracket, fields_left_square_bracket_set_right_square_bracket, filter_left_square_bracket_contains_cosmetics_only_right_square_bracket, filter_left_square_bracket_contains_cosmetics_right_square_bracket)
List Sets

Retrieve a list of sets.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**language** | **String** | a valid language code | [required] |
**game** | **String** | game main 'dofus3' or beta channel 'dofus3beta' | [required] |
**sort_left_square_bracket_level_right_square_bracket** | Option<**String**> | sort the resulting list by level, default unsorted |  |
**filter_left_square_bracket_min_highest_equipment_level_right_square_bracket** | Option<**i32**> | only results where the equipment with the highest level is above or equal to this value |  |
**filter_left_square_bracket_max_highest_equipment_level_right_square_bracket** | Option<**i32**> | only results where the equipment with the highest level is below or equal to this value |  |
**page_left_square_bracket_size_right_square_bracket** | Option<**i32**> | size of the results from the list. -1 disables pagination and gets all in one response. |  |
**page_left_square_bracket_number_right_square_bracket** | Option<**i32**> | page number based on the current page[size]. So you could get page 1 with 8 entrys and page 2 would have entries 8 to 16. |  |
**fields_left_square_bracket_set_right_square_bracket** | Option<[**Vec<String>**](String.md)> | adds fields from their detail endpoint to the item list entries. Multiple comma separated values allowed. |  |
**filter_left_square_bracket_contains_cosmetics_only_right_square_bracket** | Option<**bool**> | filter sets based on if they only got cosmetic items in it. If true, the item ids are for the cosmetic endpoints instead of equipment. |  |
**filter_left_square_bracket_contains_cosmetics_right_square_bracket** | Option<**bool**> | filter sets based on if they got cosmetic items in it. |  |

### Return type

[**models::ListEquipmentSets**](ListEquipmentSets.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_sets_search

> Vec<models::ListEquipmentSet> get_sets_search(language, game, query, filter_left_square_bracket_min_highest_equipment_level_right_square_bracket, filter_left_square_bracket_max_highest_equipment_level_right_square_bracket, limit, filter_left_square_bracket_contains_cosmetics_only_right_square_bracket, filter_left_square_bracket_contains_cosmetics_right_square_bracket)
Search Sets

Search in all names and descriptions of sets with a query.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**language** | **String** | a valid language code | [required] |
**game** | **String** | game main 'dofus3' or beta channel 'dofus3beta' | [required] |
**query** | **String** | case sensitive search query | [required] |
**filter_left_square_bracket_min_highest_equipment_level_right_square_bracket** | Option<**i32**> | only results where the equipment with the highest level is above or equal to this value |  |
**filter_left_square_bracket_max_highest_equipment_level_right_square_bracket** | Option<**i32**> | only results where the equipment with the highest level is below or equal to this value |  |
**limit** | Option<**i32**> | maximum number of returned results |  |[default to 8]
**filter_left_square_bracket_contains_cosmetics_only_right_square_bracket** | Option<**bool**> | filter sets based on if they only got cosmetic items in it. If true, the item ids are for the cosmetic endpoints instead of equipment. |  |
**filter_left_square_bracket_contains_cosmetics_right_square_bracket** | Option<**bool**> | filter sets based on if they got any cosmetic items in it |  |

### Return type

[**Vec<models::ListEquipmentSet>**](ListEquipmentSet.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_sets_single

> models::EquipmentSet get_sets_single(language, ankama_id, game)
Single Sets

Retrieve a specific set with id.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**language** | **String** | a valid language code | [required] |
**ankama_id** | **i32** | identifier | [required] |
**game** | **String** | game main 'dofus3' or beta channel 'dofus3beta' | [required] |

### Return type

[**models::EquipmentSet**](EquipmentSet.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

