# SpellScriptUsage

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ankama_id** | Option<**i32**> |  | [optional]
**script_id** | Option<**i32**> |  | [optional]
**order** | Option<**i32**> |  | [optional]
**random** | Option<**i32**> |  | [optional]
**random_group** | Option<**i32**> |  | [optional]
**sequence_group** | Option<**i32**> |  | [optional]
**activation_mask** | Option<[**models::TargetMask**](TargetMask.md)> |  | [optional]
**caster_mask** | Option<[**models::TargetMask**](TargetMask.md)> |  | [optional]
**target_mask** | Option<[**models::TargetMask**](TargetMask.md)> |  | [optional]
**activation_zone** | Option<[**models::EffectZone**](EffectZone.md)> |  | [optional]
**target_zone** | Option<[**models::EffectZone**](EffectZone.md)> |  | [optional]
**condition** | Option<**std::collections::HashMap<String, serde_json::Value>**> |  | [optional]
**targets_affected_concurrently** | Option<**bool**> |  | [optional]
**target_treated_as_caster** | Option<**bool**> |  | [optional]
**spell_level_ids** | Option<**Vec<i32>**> | Spell-level definition IDs to which this script binding applies. Match SpellLevel.ankama_id, not Spell.ankama_id or SpellLevel.grade. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


