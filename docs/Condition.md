# Condition

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**operator** | Option<**String**> | Comparison to apply to the interpreted requirement value. | [optional]
**int_value** | Option<**i32**> |  | [optional]
**element** | Option<[**models::TranslatedId**](TranslatedId.md)> |  | [optional]
**kind** | Option<**String**> | Interpreted requirement category, such as profession_level or item_received_age. Use this with the operator, values and references rather than decoding original condition tokens. | [optional]
**unit** | Option<**String**> | Unit associated with the requirement value when the interpreted condition supplies one. | [optional]
**quantity** | Option<**i32**> |  | [optional]
**string_value** | Option<**String**> |  | [optional]
**value_label** | Option<**String**> |  | [optional]
**reference** | Option<[**models::CombatReference**](CombatReference.md)> |  | [optional]
**secondary_reference** | Option<[**models::CombatReference**](CombatReference.md)> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


