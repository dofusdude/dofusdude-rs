# MonsterDrop

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**item** | [**models::CombatReference**](CombatReference.md) |  | 
**rates_percent** | [**Vec<models::MonsterDropRatesPercentInner>**](MonsterDropRatesPercentInner.md) | Base drop percentage for each monster grade. | 
**has_conditions** | **bool** |  | 
**drop_id** | Option<**i32**> |  | [optional]
**count** | Option<**i32**> |  | [optional]
**condition** | Option<**std::collections::HashMap<String, serde_json::Value>**> |  | [optional]
**hidden_if_invalid_conditions** | Option<**bool**> |  | [optional]
**disable_drop_modifier** | Option<**bool**> |  | [optional]
**specific_coefficients** | Option<**Vec<std::collections::HashMap<String, serde_json::Value>>**> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


