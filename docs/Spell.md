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
**r#type** | Option<[**models::SpellType**](SpellType.md)> |  | [optional]
**base_preview_zone** | Option<[**models::EffectZone**](EffectZone.md)> |  | [optional]
**classes** | Option<[**Vec<models::CombatReference>**](CombatReference.md)> | Reverse references to playable classes associated with this spell. These are compact references, not complete class documents. | [optional]
**monsters** | Option<[**Vec<models::CombatReference>**](CombatReference.md)> | Reverse references to monsters associated with this spell. Use a monster's grade-specific assignments to determine which spell grade it uses. | [optional]
**levels** | [**Vec<models::SpellLevel>**](SpellLevel.md) | Available spell grades. Despite the field name, entries are not player levels. A grade-filtered detail response contains only the requested entry while retaining the parent spell object. | 
**scripts** | Option<[**Vec<models::SpellScriptUsage>**](SpellScriptUsage.md)> |  | [optional]
**critical_scripts** | Option<[**Vec<models::SpellScriptUsage>**](SpellScriptUsage.md)> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


