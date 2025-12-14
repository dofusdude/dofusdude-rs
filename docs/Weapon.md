# Weapon

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ankama_id** | Option<**i32**> |  | [optional]
**name** | Option<**String**> |  | [optional]
**description** | Option<**String**> |  | [optional]
**r#type** | Option<[**models::TranslatedId**](TranslatedId.md)> |  | [optional]
**is_weapon** | Option<**bool**> | always true when the item is a weapon. Many fields are now available. Always check for this flag first when getting single equipment items. | [optional]
**level** | Option<**i32**> |  | [optional]
**pods** | Option<**i32**> |  | [optional]
**image_urls** | Option<[**models::Images**](Images.md)> |  | [optional]
**effects** | Option<[**Vec<models::Effect>**](Effect.md)> |  | [optional]
**conditions** | Option<[**models::ConditionNode**](ConditionNode.md)> |  | [optional]
**critical_hit_probability** | Option<**i32**> |  | [optional]
**critical_hit_bonus** | Option<**i32**> |  | [optional]
**max_cast_per_turn** | Option<**i32**> |  | [optional]
**ap_cost** | Option<**i32**> |  | [optional]
**range** | Option<[**models::Range**](Range.md)> |  | [optional]
**recipe** | Option<[**Vec<models::Recipe>**](Recipe.md)> |  | [optional]
**parent_set** | Option<[**models::TranslatedId**](TranslatedId.md)> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


