# \AlmanaxApi

All URIs are relative to *https://api.dofusdu.de*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_almanax_date**](AlmanaxApi.md#get_almanax_date) | **GET** /dofus3/v1/{language}/almanax/{date} | Single Almanax Date
[**get_almanax_range**](AlmanaxApi.md#get_almanax_range) | **GET** /dofus3/v1/{language}/almanax | Almanax Range



## get_almanax_date

> models::Almanax get_almanax_date(language, date, level)
Single Almanax Date

Get a single date. There are not more details in the returned object than the normal range endpoint.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**language** | **String** | code | [required] |
**date** | **String** | yyyy-mm-dd | [required] |
**level** | Option<**i32**> | character level for the reward_xp field |  |

### Return type

[**models::Almanax**](Almanax.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_almanax_range

> Vec<models::Almanax> get_almanax_range(language, filter_left_square_bracket_bonus_type_right_square_bracket, range_left_square_bracket_from_right_square_bracket, range_left_square_bracket_to_right_square_bracket, range_left_square_bracket_size_right_square_bracket, timezone, level)
Almanax Range

Get a range of dates, defaults to today + 6 following days but can specified by the query parameters.   filter[bonus_type] can be used seperately and does not have an effect on the other parameters.  range[from] changes the start date, everything else defaults to 6 following dates from this start date.  range[to] when used without anything else, it will use today as start date and this parameter as end. All ranges are inclusive.  range[from] + range[to] = inclusive range over the specified dates, should never be farther apart than 35 days.  range[from|to] + range[size] no need to specify the date, just following days with [from] (0 is today) or go backwards in time with only [to] and [size].  Not all combinations are listed but this should give you an idea how to they could work.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**language** | **String** | code | [required] |
**filter_left_square_bracket_bonus_type_right_square_bracket** | Option<**String**> | ids from meta/{language}/almanax/bonuses |  |
**range_left_square_bracket_from_right_square_bracket** | Option<**String**> | yyyy-mm-dd |  |
**range_left_square_bracket_to_right_square_bracket** | Option<**String**> | yyyy-mm-dd |  |
**range_left_square_bracket_size_right_square_bracket** | Option<**i32**> | Size of the returned range. Disable to fully use the range by setting size to -1. |  |
**timezone** | Option<**String**> | determine what the current time is. If you live in Brazil, \"today\" will be hours apart from Paris. Use your timezone to get results relative to your location. |  |[default to Europe/Paris]
**level** | Option<**i32**> | character level for the reward_xp field |  |

### Return type

[**Vec<models::Almanax>**](Almanax.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

