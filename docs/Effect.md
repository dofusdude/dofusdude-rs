# Effect

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**int_minimum** | Option<**i32**> | minimum int value, can be a single if ignore_int_max and no ignore_int_min | [optional]
**int_maximum** | Option<**i32**> | maximum int value, if not ignore_int_max and not ignore_int_min, the effect has a range value | [optional]
**r#type** | Option<[**models::EffectType**](EffectType.md)> |  | [optional]
**ignore_int_min** | Option<**bool**> | ignore the int min field because the actual value is a string. For readability the templated field is the only important field in this case.  | [optional]
**ignore_int_max** | Option<**bool**> | ignore the int max field, if ignore_int_min is true, int min is a single value | [optional]
**formatted** | Option<**String**> | all fields from above encoded in a single string | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


