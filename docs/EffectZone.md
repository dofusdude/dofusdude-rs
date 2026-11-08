# EffectZone

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**raw** | Option<**String**> | Original compact zone encoding when the source provides one. | [optional]
**shape** | [**models::ZoneShape**](ZoneShape.md) |  | 
**size** | Option<**i32**> | Effective outer size of the area. A point has size 0; whole-map and custom-cell shapes omit it. | [optional]
**min_size** | Option<**i32**> | Effective inner size for hollow or minimum-size shapes. Omitted when the shape has no inner boundary. | [optional]
**cell_ids** | **Vec<i32>** |  | 
**damage_decrease_step_percent** | Option<**i32**> |  | [optional]
**max_damage_decrease_apply_count** | Option<**i32**> |  | [optional]
**forced_direction** | Option<**i32**> |  | [optional]
**include_carried** | Option<**bool**> |  | [optional]
**stop_at_target** | Option<**bool**> |  | [optional]
**only_affect_in_sight_line** | Option<**bool**> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


