# Monster

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ankama_id** | **i32** |  | 
**name** | **String** |  | 
**image_urls** | Option<[**models::Images**](Images.md)> |  | [optional]
**race** | [**models::MonsterRace**](MonsterRace.md) |  | 
**grades** | [**Vec<models::MonsterGrade>**](MonsterGrade.md) | Variants of this monster. Each has its own combat level, statistics and assigned spells. The monster grade number is not a spell grade number or combat level. | 
**spawn_locations** | [**Vec<models::MonsterSpawnLocation>**](MonsterSpawnLocation.md) | Known spawn subareas and their geographic parents. This is not live population data or a per-map spawn probability. Maps listed within a subarea are not guaranteed individual spawn points. | 
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


