# SpellEffect

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**r#type** | Option<**String**> | Localized effect category, such as Air damage. This is not a spell ID or a structured game reference. | [optional]
**min** | Option<**i32**> |  | [optional]
**max** | Option<**i32**> |  | [optional]
**duration** | Option<**i32**> | Effect duration in fight turns as represented by the source. Not a real-time duration in seconds. | [optional]
**delay** | Option<**i32**> | Delay before the effect in fight turns as represented by the source. | [optional]
**random** | Option<**f64**> | Source random-selection value. Do not interpret it as a percentage without the effect's selection rules. | [optional]
**group** | Option<**i32**> |  | [optional]
**dispellable** | Option<**i32**> |  | [optional]
**effect_uid** | Option<**i32**> | Stable identifier of this concrete effect instance. | [optional]
**target_id** | Option<**i32**> |  | [optional]
**triggered_duration** | Option<**i32**> |  | [optional]
**display_zero** | Option<**bool**> |  | [optional]
**modifier** | Option<**i32**> |  | [optional]
**zone** | Option<[**models::EffectZone**](EffectZone.md)> |  | [optional]
**target_mask** | Option<[**models::TargetMask**](TargetMask.md)> |  | [optional]
**triggers** | Option<[**models::SpellTriggers**](SpellTriggers.md)> |  | [optional]
**templated** | Option<**String**> | Localized effect text suitable for display. Numeric effect properties remain available separately. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


