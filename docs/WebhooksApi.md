# \WebhooksApi

All URIs are relative to *https://api.dofusdu.de*

Method | HTTP request | Description
------------- | ------------- | -------------
[**delete_webhooks_almanax_id**](WebhooksApi.md#delete_webhooks_almanax_id) | **DELETE** /webhooks/almanax/{id} | Unregister Almanax Hook
[**delete_webhooks_rss_id**](WebhooksApi.md#delete_webhooks_rss_id) | **DELETE** /webhooks/rss/{id} | Unregister RSS Hook
[**delete_webhooks_twitter_id**](WebhooksApi.md#delete_webhooks_twitter_id) | **DELETE** /webhooks/twitter/{id} | Unregister Twitter Hook
[**get_meta_webhooks_almanax**](WebhooksApi.md#get_meta_webhooks_almanax) | **GET** /meta/webhooks/almanax | Get Almanax Hook Metainfo
[**get_meta_webhooks_rss**](WebhooksApi.md#get_meta_webhooks_rss) | **GET** /meta/webhooks/rss | Get RSS Hook Metainfo
[**get_meta_webhooks_twitter**](WebhooksApi.md#get_meta_webhooks_twitter) | **GET** /meta/webhooks/twitter | Get Twitter Hook Metainfo
[**get_webhooks_almanax_id**](WebhooksApi.md#get_webhooks_almanax_id) | **GET** /webhooks/almanax/{id} | Get Almanax Hook
[**get_webhooks_rss_id**](WebhooksApi.md#get_webhooks_rss_id) | **GET** /webhooks/rss/{id} | Get RSS Hook
[**get_webhooks_twitter_id**](WebhooksApi.md#get_webhooks_twitter_id) | **GET** /webhooks/twitter/{id} | Get Twitter Hook
[**post_webhooks_almanax**](WebhooksApi.md#post_webhooks_almanax) | **POST** /webhooks/almanax | Register Almanax Hook
[**post_webhooks_rss**](WebhooksApi.md#post_webhooks_rss) | **POST** /webhooks/rss | Register RSS Hook
[**post_webhooks_twitter**](WebhooksApi.md#post_webhooks_twitter) | **POST** /webhooks/twitter | Register Twitter Hook
[**put_webhooks_almanax_id**](WebhooksApi.md#put_webhooks_almanax_id) | **PUT** /webhooks/almanax/{id} | Update Almanax Hook
[**put_webhooks_rss_id**](WebhooksApi.md#put_webhooks_rss_id) | **PUT** /webhooks/rss/{id} | Update RSS Hook
[**put_webhooks_twitter_id**](WebhooksApi.md#put_webhooks_twitter_id) | **PUT** /webhooks/twitter/{id} | Update Twitter Hook



## delete_webhooks_almanax_id

> delete_webhooks_almanax_id(id)
Unregister Almanax Hook

Delete a Webhook from the service.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **String** | the ID returned from the API when creating the webhook | [required] |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_webhooks_rss_id

> delete_webhooks_rss_id(id)
Unregister RSS Hook

Delete a Webhook from the service.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **String** | the ID returned from the API when creating the webhook | [required] |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_webhooks_twitter_id

> delete_webhooks_twitter_id(id)
Unregister Twitter Hook

Delete a Webhook from the service.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **String** | the ID returned from the API when creating the webhook | [required] |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_meta_webhooks_almanax

> models::GetMetaWebhooksTwitter200Response get_meta_webhooks_almanax()
Get Almanax Hook Metainfo

Get a list of all available subscriptions. 

### Parameters

This endpoint does not need any parameter.

### Return type

[**models::GetMetaWebhooksTwitter200Response**](get_meta_webhooks_twitter_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_meta_webhooks_rss

> models::GetMetaWebhooksTwitter200Response get_meta_webhooks_rss()
Get RSS Hook Metainfo

Get a list of all available subscriptions. 

### Parameters

This endpoint does not need any parameter.

### Return type

[**models::GetMetaWebhooksTwitter200Response**](get_meta_webhooks_twitter_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_meta_webhooks_twitter

> models::GetMetaWebhooksTwitter200Response get_meta_webhooks_twitter()
Get Twitter Hook Metainfo

Get a list of all available subscriptions. 

### Parameters

This endpoint does not need any parameter.

### Return type

[**models::GetMetaWebhooksTwitter200Response**](get_meta_webhooks_twitter_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_webhooks_almanax_id

> models::AlmanaxWebhook get_webhooks_almanax_id(id)
Get Almanax Hook

Retrieve details about an existing Almanax Webhook with a given uuid.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **String** | the ID returned from the API when creating the webhook | [required] |

### Return type

[**models::AlmanaxWebhook**](AlmanaxWebhook.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_webhooks_rss_id

> models::RssWebhook get_webhooks_rss_id(id)
Get RSS Hook

Retrieve details about an existing RSS Webhook with a given uuid.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **String** | the ID returned from the API when creating the webhook | [required] |

### Return type

[**models::RssWebhook**](RssWebhook.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_webhooks_twitter_id

> models::TwitterWebhook get_webhooks_twitter_id(id)
Get Twitter Hook

Retrieve details about an existing Twitter Webhook with a given uuid.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **String** | the ID returned from the API when creating the webhook | [required] |

### Return type

[**models::TwitterWebhook**](TwitterWebhook.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## post_webhooks_almanax

> post_webhooks_almanax(create_almanax_webhook)
Register Almanax Hook

Register a new Webhook to post Almanax updates.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_almanax_webhook** | Option<[**CreateAlmanaxWebhook**](CreateAlmanaxWebhook.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## post_webhooks_rss

> post_webhooks_rss(create_rss_webhook)
Register RSS Hook

Register a new Webhook to post RSS news as soon as they are posted.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_rss_webhook** | Option<[**CreateRssWebhook**](CreateRssWebhook.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## post_webhooks_twitter

> post_webhooks_twitter(create_twitter_webhook)
Register Twitter Hook

Register a new Webhook to post Twitter updates as soon as they are posted.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_twitter_webhook** | Option<[**CreateTwitterWebhook**](CreateTwitterWebhook.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## put_webhooks_almanax_id

> models::AlmanaxWebhook put_webhooks_almanax_id(id, put_almanax_webhook)
Update Almanax Hook

Update the details of an Almanax Webhook. All fields are optional and arrays will be overwritten, so always put all selected items of an array.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **String** | the ID returned from the API when creating the webhook | [required] |
**put_almanax_webhook** | Option<[**PutAlmanaxWebhook**](PutAlmanaxWebhook.md)> |  |  |

### Return type

[**models::AlmanaxWebhook**](AlmanaxWebhook.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## put_webhooks_rss_id

> models::RssWebhook put_webhooks_rss_id(id, put_rss_webhook)
Update RSS Hook

Update the details of a RSS Webhook. All fields are optional and arrays will be overwritten, so always put all selected items of an array.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **String** | the ID returned from the API when creating the webhook | [required] |
**put_rss_webhook** | Option<[**PutRssWebhook**](PutRssWebhook.md)> |  |  |

### Return type

[**models::RssWebhook**](RssWebhook.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## put_webhooks_twitter_id

> models::TwitterWebhook put_webhooks_twitter_id(id, put_twitter_webhook)
Update Twitter Hook

Update the details of a Twitter Webhook. All fields are optional and arrays will be overwritten, so always put all selected items of an array.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **String** | the ID returned from the API when creating the webhook | [required] |
**put_twitter_webhook** | Option<[**PutTwitterWebhook**](PutTwitterWebhook.md)> |  |  |

### Return type

[**models::TwitterWebhook**](TwitterWebhook.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

