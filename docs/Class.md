# Class

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ankama_id** | **i32** |  | 
**name** | **String** |  | 
**description** | Option<**String**> |  | [optional]
**gameplay_description** | Option<**String**> |  | [optional]
**complexity** | Option<**i32**> |  | [optional]
**sort_index** | Option<**i32**> |  | [optional]
**creature_bones_id** | Option<**i32**> |  | [optional]
**roles** | Option<**Vec<std::collections::HashMap<String, serde_json::Value>>**> |  | [optional]
**characteristic_costs** | Option<[**std::collections::HashMap<String, Vec<models::ClassCharacteristicCostsValueInner>>**](Vec.md)> | Characteristic point-cost tiers keyed by characteristic name. | [optional]
**image_urls** | Option<[**models::Images**](Images.md)> |  | [optional]
**looks** | [**models::ClassLooks**](ClassLooks.md) |  | 
**spells** | [**Vec<models::Spell>**](Spell.md) | Full spell definitions assigned to this playable class, including their own grades, effects and targeting. A class has no monster-grade dimension. The same spells are independently available from the spells endpoint. | 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


