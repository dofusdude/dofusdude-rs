# Monster

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ankama_id** | **i32** |  | 
**name** | **String** |  | 
**image_urls** | Option<[**models::Images**](Images.md)> |  | [optional]
**race** | [**models::MonsterRace**](MonsterRace.md) |  | 
**grades** | [**Vec<models::MonsterGrade>**](MonsterGrade.md) | Monster statistics and spells grouped by the monster grade that uses them. | 
**spawn_locations** | [**Vec<models::MonsterSpawnLocation>**](MonsterSpawnLocation.md) | Spawn subareas taken from the monster's authoritative subarea list. | 
**drops** | [**Vec<models::MonsterDrop>**](MonsterDrop.md) |  | 
**global_drops** | Option<[**Vec<models::MonsterGlobalDrop>**](MonsterGlobalDrop.md)> |  | [optional]
**appearance** | Option<[**models::ClassAppearance**](ClassAppearance.md)> |  | [optional]
**is_bounty** | Option<**bool**> |  | [optional]
**corresponding_mini_boss** | Option<[**models::CombatReference**](CombatReference.md)> |  | [optional]
**summon_cost** | Option<**i32**> |  | [optional]
**speed_adjust** | Option<**i32**> |  | [optional]
**scale_grade_reference** | Option<**i32**> |  | [optional]
**achievements** | Option<[**Vec<models::CombatReference>**](CombatReference.md)> |  | [optional]
**souls** | Option<**Vec<std::collections::HashMap<String, serde_json::Value>>**> |  | [optional]
**characteristic_ratios** | Option<[**Vec<Vec<f64>>**](Vec.md)> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


