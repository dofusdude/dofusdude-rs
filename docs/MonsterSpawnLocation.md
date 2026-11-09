# MonsterSpawnLocation

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**subarea** | [**models::CombatReference**](CombatReference.md) |  | 
**area** | [**models::CombatReference**](CombatReference.md) |  | 
**super_area** | [**models::CombatReference**](CombatReference.md) |  | 
**subarea_maps** | [**Vec<models::MonsterSpawnLocationSubareaMapsInner>**](MonsterSpawnLocationSubareaMapsInner.md) | Maps belonging to the referenced subarea. Map membership alone is not proof that the monster spawns on a particular map. | 
**preferred** | **bool** | Whether the source marks this as a preferred subarea. A preference flag, not a spawn percentage or guarantee of presence. | 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


