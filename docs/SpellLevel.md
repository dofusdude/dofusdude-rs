# SpellLevel

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ankama_id** | Option<**i32**> | ID of the spell-level definition. Different from the parent spell ID and from the grade number. Used by explicit spell-level references such as script spell_level_ids. | [optional]
**grade** | Option<**i32**> | Number identifying this variant within its spell. Select by this value, not by the array position. Used by the spell detail endpoint's grade parameter. | [optional]
**ap_cost** | Option<**i32**> | Action points required to cast this spell grade. | [optional]
**critical_hit_probability** | Option<**i32**> | Base critical-hit percentage recorded for this spell grade, before fighter-specific modifiers. | [optional]
**min_player_level** | Option<**i32**> | Player-level requirement recorded for this spell grade. This is not its grade number or a monster combat level. | [optional]
**min_range** | Option<**i32**> | Minimum casting range in combat cells. | [optional]
**max_range** | Option<**i32**> | Maximum casting range in combat cells as defined by this grade. | [optional]
**max_cast_per_turn** | Option<**i32**> | Per-caster cast limit within a turn as recorded by the source. | [optional]
**max_cast_per_target** | Option<**i32**> |  | [optional]
**max_global_cast_per_turn** | Option<**i32**> |  | [optional]
**max_global_cast_per_target** | Option<**i32**> |  | [optional]
**min_cast_interval** | Option<**i32**> | Minimum interval between casts, measured in fight turns. | [optional]
**initial_cooldown** | Option<**i32**> | Initial wait before casting, measured in fight turns. | [optional]
**global_cooldown** | Option<**i32**> |  | [optional]
**ignore_prison_glyph** | Option<**bool**> |  | [optional]
**spell_breed** | Option<**i32**> |  | [optional]
**states_criterion** | Option<[**models::EligibilityNode**](EligibilityNode.md)> | Available client-side state requirements for this spell grade. Null does not assert that the server imposes no restriction. | [optional]
**preview_zones** | Option<[**Vec<models::SpellPreviewZone>**](SpellPreviewZone.md)> | Client preview and activation geometry for this grade. Use each effect's zone for its actual effect-area definition. | [optional]
**effects** | Option<[**Vec<models::SpellEffect>**](SpellEffect.md)> | Normal-cast effects for this grade. Each entry has independent targeting and area geometry. | [optional]
**critical_effects** | Option<[**Vec<models::SpellEffect>**](SpellEffect.md)> | Critical-cast effects for this grade. Keep separate from normal effects rather than applying both arrays to every cast. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


