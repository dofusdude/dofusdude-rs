# WorldArea

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ankama_id** | **i32** |  | 
**name** | **String** |  | 
**world_map_id** | Option<**i32**> | World-map context supplied on super-area records. | [optional]
**areas** | Option<[**Vec<models::CombatReference>**](CombatReference.md)> | Child area references supplied on super-area records. | [optional]
**level** | Option<**i32**> | Suggested geographic difficulty level supplied on subarea records. Not a monster grade or the level of every monster there. | [optional]
**dungeon_id** | Option<**i32**> | Dungeon association when supplied by the subarea data. | [optional]
**maps** | Option<[**Vec<models::WorldMapReference>**](WorldMapReference.md)> | Map membership supplied on subarea records. Does not imply a spawn on every map. | [optional]
**super_area** | Option<[**models::CombatReference**](CombatReference.md)> |  | [optional]
**area** | Option<[**models::CombatReference**](CombatReference.md)> |  | [optional]
**subareas** | Option<[**Vec<models::CombatReference>**](CombatReference.md)> |  | [optional]
**monsters** | Option<[**Vec<models::CombatReference>**](CombatReference.md)> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


