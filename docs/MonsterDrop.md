# MonsterDrop

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**item** | [**models::CombatReference**](CombatReference.md) |  | 
**rates_percent** | [**Vec<models::MonsterDropRatesPercentInner>**](MonsterDropRatesPercentInner.md) | Base drop percentages indexed by MonsterGrade.grade, not spell grade or array position. A value of 5 means 5 percent, not 0.05 percent. These are not spawn percentages. | 
**has_conditions** | **bool** | The source reports restrictions. Can be true without a complete client-side condition tree because server-only predicates are not exposed. | 
**drop_id** | Option<**i32**> |  | [optional]
**count** | Option<**i32**> |  | [optional]
**condition** | Option<**std::collections::HashMap<String, serde_json::Value>**> |  | [optional]
**hidden_if_invalid_conditions** | Option<**bool**> |  | [optional]
**disable_drop_modifier** | Option<**bool**> |  | [optional]
**specific_coefficients** | Option<**Vec<std::collections::HashMap<String, serde_json::Value>>**> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


