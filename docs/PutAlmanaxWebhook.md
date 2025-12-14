# PutAlmanaxWebhook

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**bonus_whitelist** | Option<**Vec<String>**> | from all available bonuses (ids) from /dofus3/meta/{language}/almanax/bonuses. Delete old entries with empty array []. Just null changes nothing. | [optional]
**bonus_blacklist** | Option<**Vec<String>**> | from all available bonuses (ids) from /dofus3/meta/{language}/almanax/bonuses. Delete old entries with empty array []. Just null changes nothing. | [optional]
**subscriptions** | Option<**Vec<String>**> | Get the available subscriptions with /meta/webhooks/almanax | [optional]
**daily_settings** | Option<[**models::CreateAlmanaxWebhookDailySettings**](CreateAlmanaxWebhook_daily_settings.md)> |  | [optional]
**iso_date** | Option<**bool**> | If false, it will use common local time formats and weekday translations. If true, the format is YYYY-MM-DD. | [optional][default to false]
**mentions** | Option<[**std::collections::HashMap<String, Vec<models::CreateAlmanaxWebhookMentionsValueInner>>**](Vec.md)> | Almanax bonus ids mapped to array of mentions. | [optional]
**intervals** | Option<**Vec<String>**> |  | [optional]
**weekly_weekday** | Option<**String**> | When to post the weekly preview at the specified time. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


