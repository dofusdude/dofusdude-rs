# \MetaApi

All URIs are relative to *https://api.dofusdu.de*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_game_search_types**](MetaApi.md#get_game_search_types) | **GET** /{game}/v1/meta/search/types | Available Game Search Types
[**get_item_types**](MetaApi.md#get_item_types) | **GET** /{game}/v1/meta/items/types | Available Item Types
[**get_meta_almanax_bonuses**](MetaApi.md#get_meta_almanax_bonuses) | **GET** /dofus3/v1/meta/{language}/almanax/bonuses | Available Almanax Bonuses
[**get_meta_almanax_bonuses_search**](MetaApi.md#get_meta_almanax_bonuses_search) | **GET** /dofus3/v1/meta/{language}/almanax/bonuses/search | Search Available Almanax Bonuses
[**get_meta_elements**](MetaApi.md#get_meta_elements) | **GET** /{game}/v1/meta/elements | Effects and Condition Elements
[**get_meta_version**](MetaApi.md#get_meta_version) | **GET** /{game}/v1/meta/version | Game Version



## get_game_search_types

> Vec<String> get_game_search_types(game)
Available Game Search Types

Get all types for /{game}/v1/{lang}/search available for filtering. All names are english for comparing them inside applications. Order is fixed so you can compare indices instead of strings.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**game** | **String** | game main 'dofus3' or beta channel 'dofus3beta' | [required] |

### Return type

**Vec<String>**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_item_types

> Vec<String> get_item_types(game)
Available Item Types

Get all types of all items. Primarily used for filtering more detailed types in listings or search endpoints. All names are english for comparing them inside applications. Ordering is not guaranteed to persist with game updates.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**game** | **String** | game main 'dofus3' or beta channel 'dofus3beta' | [required] |

### Return type

**Vec<String>**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_meta_almanax_bonuses

> Vec<models::GetMetaAlmanaxBonuses200ResponseInner> get_meta_almanax_bonuses(language)
Available Almanax Bonuses

Get all the available bonuses and their id for filtering them in the range endpoint.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**language** | **String** | a valid language code | [required] |

### Return type

[**Vec<models::GetMetaAlmanaxBonuses200ResponseInner>**](get_meta_almanax_bonuses_200_response_inner.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_meta_almanax_bonuses_search

> Vec<models::GetMetaAlmanaxBonuses200ResponseInner> get_meta_almanax_bonuses_search(language, query, limit)
Search Available Almanax Bonuses

Search all the available bonuses and their id for filtering them in the range endpoint.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**language** | **String** | a valid language code | [required] |
**query** | **String** | case sensitive search query | [required] |
**limit** | Option<**i32**> | maximum number of returned results |  |

### Return type

[**Vec<models::GetMetaAlmanaxBonuses200ResponseInner>**](get_meta_almanax_bonuses_200_response_inner.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_meta_elements

> Vec<String> get_meta_elements(game)
Effects and Condition Elements

Get the mappings for all specific elements that are linked in the dataset. All names are english. Translations are not needed because of a global unique id which is the index inside the array. Future elements will get a higher id.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**game** | **String** | game main 'dofus3' or beta channel 'dofus3beta' | [required] |

### Return type

**Vec<String>**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_meta_version

> models::Version get_meta_version(game)
Game Version

The current game version of the hosted data.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**game** | **String** | game main 'dofus3' or beta channel 'dofus3beta' | [required] |

### Return type

[**models::Version**](Version.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

