# Spell

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ankama_id** | **i32** |  | 
**name** | **String** |  | 
**description** | Option<**String**> |  | [optional]
**icon_id** | Option<**i32**> |  | [optional]
**admin_name** | Option<**String**> |  | [optional]
**order** | Option<**i32**> |  | [optional]
**image_urls** | Option<[**models::Images**](Images.md)> |  | [optional]
**r#type** | Option<[**models::CombatReference**](CombatReference.md)> |  | [optional]
**classes** | Option<[**Vec<models::CombatReference>**](CombatReference.md)> |  | [optional]
**monsters** | Option<[**Vec<models::CombatReference>**](CombatReference.md)> |  | [optional]
**levels** | [**Vec<models::SpellLevel>**](SpellLevel.md) |  | 
**scripts** | Option<[**Vec<models::SpellScriptUsage>**](SpellScriptUsage.md)> |  | [optional]
**critical_scripts** | Option<[**Vec<models::SpellScriptUsage>**](SpellScriptUsage.md)> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


