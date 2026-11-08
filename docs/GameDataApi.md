# \GameDataApi

All URIs are relative to *https://api.dofusdu.de*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_all_areas**](GameDataApi.md#get_all_areas) | **GET** /{game}/v1/{language}/areas/all | Get all areas
[**get_all_classes**](GameDataApi.md#get_all_classes) | **GET** /{game}/v1/{language}/classes/all | Get all classes
[**get_all_monsters**](GameDataApi.md#get_all_monsters) | **GET** /{game}/v1/{language}/monsters/all | Get all monsters
[**get_all_spells**](GameDataApi.md#get_all_spells) | **GET** /{game}/v1/{language}/spells/all | Get all spells
[**get_all_subareas**](GameDataApi.md#get_all_subareas) | **GET** /{game}/v1/{language}/subareas/all | Get all subareas
[**get_all_super_areas**](GameDataApi.md#get_all_super_areas) | **GET** /{game}/v1/{language}/super-areas/all | Get all super-areas
[**get_area_by_id**](GameDataApi.md#get_area_by_id) | **GET** /{game}/v1/{language}/areas/{ankama_id} | Get one area
[**get_areas**](GameDataApi.md#get_areas) | **GET** /{game}/v1/{language}/areas | List areas
[**get_class_by_id**](GameDataApi.md#get_class_by_id) | **GET** /{game}/v1/{language}/classes/{ankama_id} | Get one class
[**get_classes**](GameDataApi.md#get_classes) | **GET** /{game}/v1/{language}/classes | List classes
[**get_monster_by_id**](GameDataApi.md#get_monster_by_id) | **GET** /{game}/v1/{language}/monsters/{ankama_id} | Get one monster
[**get_monsters**](GameDataApi.md#get_monsters) | **GET** /{game}/v1/{language}/monsters | List monsters
[**get_spell_by_id**](GameDataApi.md#get_spell_by_id) | **GET** /{game}/v1/{language}/spells/{ankama_id} | Get one spell
[**get_spells**](GameDataApi.md#get_spells) | **GET** /{game}/v1/{language}/spells | List spells
[**get_subarea_by_id**](GameDataApi.md#get_subarea_by_id) | **GET** /{game}/v1/{language}/subareas/{ankama_id} | Get one subarea
[**get_subareas**](GameDataApi.md#get_subareas) | **GET** /{game}/v1/{language}/subareas | List subareas
[**get_super_area_by_id**](GameDataApi.md#get_super_area_by_id) | **GET** /{game}/v1/{language}/super-areas/{ankama_id} | Get one super-area
[**get_super_areas**](GameDataApi.md#get_super_areas) | **GET** /{game}/v1/{language}/super-areas | List super-areas
[**search_areas**](GameDataApi.md#search_areas) | **GET** /{game}/v1/{language}/areas/search | Search areas
[**search_classes**](GameDataApi.md#search_classes) | **GET** /{game}/v1/{language}/classes/search | Search classes
[**search_monsters**](GameDataApi.md#search_monsters) | **GET** /{game}/v1/{language}/monsters/search | Search monsters
[**search_spells**](GameDataApi.md#search_spells) | **GET** /{game}/v1/{language}/spells/search | Search spells
[**search_subareas**](GameDataApi.md#search_subareas) | **GET** /{game}/v1/{language}/subareas/search | Search subareas
[**search_super_areas**](GameDataApi.md#search_super_areas) | **GET** /{game}/v1/{language}/super-areas/search | Search super-areas



## get_all_areas

> models::MappedEntityCollection get_all_areas(game, language)
Get all areas

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**game** | **String** |  | [required] |
**language** | **String** |  | [required] |

### Return type

[**models::MappedEntityCollection**](MappedEntityCollection.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_all_classes

> models::MappedEntityCollection get_all_classes(game, language)
Get all classes

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**game** | **String** |  | [required] |
**language** | **String** |  | [required] |

### Return type

[**models::MappedEntityCollection**](MappedEntityCollection.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_all_monsters

> models::MappedEntityCollection get_all_monsters(game, language, include)
Get all monsters

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**game** | **String** |  | [required] |
**language** | **String** |  | [required] |
**include** | Option<**String**> | Optional spell expansion for monster responses. Leave include unset to return spell URLs. Use `spells.grade` to embed the assigned spell grade. Use `spells` to embed every available grade of each assigned spell. |  |

### Return type

[**models::MappedEntityCollection**](MappedEntityCollection.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_all_spells

> models::MappedEntityCollection get_all_spells(game, language)
Get all spells

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**game** | **String** |  | [required] |
**language** | **String** |  | [required] |

### Return type

[**models::MappedEntityCollection**](MappedEntityCollection.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_all_subareas

> models::MappedEntityCollection get_all_subareas(game, language)
Get all subareas

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**game** | **String** |  | [required] |
**language** | **String** |  | [required] |

### Return type

[**models::MappedEntityCollection**](MappedEntityCollection.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_all_super_areas

> models::MappedEntityCollection get_all_super_areas(game, language)
Get all super-areas

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**game** | **String** |  | [required] |
**language** | **String** |  | [required] |

### Return type

[**models::MappedEntityCollection**](MappedEntityCollection.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_area_by_id

> models::WorldArea get_area_by_id(game, language, ankama_id)
Get one area

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**game** | **String** |  | [required] |
**language** | **String** |  | [required] |
**ankama_id** | **i32** |  | [required] |

### Return type

[**models::WorldArea**](WorldArea.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_areas

> models::MappedEntityCollection get_areas(game, language, page_left_square_bracket_number_right_square_bracket, page_left_square_bracket_size_right_square_bracket, fields_left_square_bracket_areas_right_square_bracket)
List areas

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**game** | **String** |  | [required] |
**language** | **String** |  | [required] |
**page_left_square_bracket_number_right_square_bracket** | Option<**i32**> |  |  |[default to 1]
**page_left_square_bracket_size_right_square_bracket** | Option<**i32**> |  |  |[default to 20]
**fields_left_square_bracket_areas_right_square_bracket** | Option<**String**> |  |  |

### Return type

[**models::MappedEntityCollection**](MappedEntityCollection.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_class_by_id

> models::Class get_class_by_id(game, language, ankama_id)
Get one class

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**game** | **String** |  | [required] |
**language** | **String** |  | [required] |
**ankama_id** | **i32** |  | [required] |

### Return type

[**models::Class**](Class.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_classes

> models::MappedEntityCollection get_classes(game, language, page_left_square_bracket_number_right_square_bracket, page_left_square_bracket_size_right_square_bracket, fields_left_square_bracket_classes_right_square_bracket)
List classes

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**game** | **String** |  | [required] |
**language** | **String** |  | [required] |
**page_left_square_bracket_number_right_square_bracket** | Option<**i32**> |  |  |[default to 1]
**page_left_square_bracket_size_right_square_bracket** | Option<**i32**> |  |  |[default to 20]
**fields_left_square_bracket_classes_right_square_bracket** | Option<**String**> |  |  |

### Return type

[**models::MappedEntityCollection**](MappedEntityCollection.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_monster_by_id

> models::Monster get_monster_by_id(game, language, ankama_id, include)
Get one monster

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**game** | **String** |  | [required] |
**language** | **String** |  | [required] |
**ankama_id** | **i32** |  | [required] |
**include** | Option<**String**> | Optional spell expansion for monster responses. Leave include unset to return spell URLs. Use `spells.grade` to embed the assigned spell grade. Use `spells` to embed every available grade of each assigned spell. |  |

### Return type

[**models::Monster**](Monster.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_monsters

> models::MappedEntityCollection get_monsters(game, language, page_left_square_bracket_number_right_square_bracket, page_left_square_bracket_size_right_square_bracket, fields_left_square_bracket_monsters_right_square_bracket, include)
List monsters

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**game** | **String** |  | [required] |
**language** | **String** |  | [required] |
**page_left_square_bracket_number_right_square_bracket** | Option<**i32**> |  |  |[default to 1]
**page_left_square_bracket_size_right_square_bracket** | Option<**i32**> |  |  |[default to 20]
**fields_left_square_bracket_monsters_right_square_bracket** | Option<**String**> |  |  |
**include** | Option<**String**> | Optional spell expansion for monster responses. Leave include unset to return spell URLs. Use `spells.grade` to embed the assigned spell grade. Use `spells` to embed every available grade of each assigned spell. |  |

### Return type

[**models::MappedEntityCollection**](MappedEntityCollection.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_spell_by_id

> models::Spell get_spell_by_id(game, language, ankama_id, grade)
Get one spell

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**game** | **String** |  | [required] |
**language** | **String** |  | [required] |
**ankama_id** | **i32** |  | [required] |
**grade** | Option<**i32**> | Return only the requested mapped spell grade in `levels`. |  |

### Return type

[**models::Spell**](Spell.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_spells

> models::MappedEntityCollection get_spells(game, language, page_left_square_bracket_number_right_square_bracket, page_left_square_bracket_size_right_square_bracket, fields_left_square_bracket_spells_right_square_bracket)
List spells

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**game** | **String** |  | [required] |
**language** | **String** |  | [required] |
**page_left_square_bracket_number_right_square_bracket** | Option<**i32**> |  |  |[default to 1]
**page_left_square_bracket_size_right_square_bracket** | Option<**i32**> |  |  |[default to 20]
**fields_left_square_bracket_spells_right_square_bracket** | Option<**String**> |  |  |

### Return type

[**models::MappedEntityCollection**](MappedEntityCollection.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_subarea_by_id

> models::WorldArea get_subarea_by_id(game, language, ankama_id)
Get one subarea

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**game** | **String** |  | [required] |
**language** | **String** |  | [required] |
**ankama_id** | **i32** |  | [required] |

### Return type

[**models::WorldArea**](WorldArea.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_subareas

> models::MappedEntityCollection get_subareas(game, language, page_left_square_bracket_number_right_square_bracket, page_left_square_bracket_size_right_square_bracket, fields_left_square_bracket_subareas_right_square_bracket)
List subareas

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**game** | **String** |  | [required] |
**language** | **String** |  | [required] |
**page_left_square_bracket_number_right_square_bracket** | Option<**i32**> |  |  |[default to 1]
**page_left_square_bracket_size_right_square_bracket** | Option<**i32**> |  |  |[default to 20]
**fields_left_square_bracket_subareas_right_square_bracket** | Option<**String**> |  |  |

### Return type

[**models::MappedEntityCollection**](MappedEntityCollection.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_super_area_by_id

> models::WorldArea get_super_area_by_id(game, language, ankama_id)
Get one super-area

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**game** | **String** |  | [required] |
**language** | **String** |  | [required] |
**ankama_id** | **i32** |  | [required] |

### Return type

[**models::WorldArea**](WorldArea.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_super_areas

> models::MappedEntityCollection get_super_areas(game, language, page_left_square_bracket_number_right_square_bracket, page_left_square_bracket_size_right_square_bracket, fields_left_square_bracket_super_areas_right_square_bracket)
List super-areas

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**game** | **String** |  | [required] |
**language** | **String** |  | [required] |
**page_left_square_bracket_number_right_square_bracket** | Option<**i32**> |  |  |[default to 1]
**page_left_square_bracket_size_right_square_bracket** | Option<**i32**> |  |  |[default to 20]
**fields_left_square_bracket_super_areas_right_square_bracket** | Option<**String**> |  |  |

### Return type

[**models::MappedEntityCollection**](MappedEntityCollection.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## search_areas

> Vec<models::MappedEntityListEntry> search_areas(game, language, query, limit)
Search areas

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**game** | **String** |  | [required] |
**language** | **String** |  | [required] |
**query** | **String** |  | [required] |
**limit** | Option<**i32**> |  |  |[default to 8]

### Return type

[**Vec<models::MappedEntityListEntry>**](MappedEntityListEntry.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## search_classes

> Vec<models::MappedEntityListEntry> search_classes(game, language, query, limit)
Search classes

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**game** | **String** |  | [required] |
**language** | **String** |  | [required] |
**query** | **String** |  | [required] |
**limit** | Option<**i32**> |  |  |[default to 8]

### Return type

[**Vec<models::MappedEntityListEntry>**](MappedEntityListEntry.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## search_monsters

> Vec<models::MappedEntityListEntry> search_monsters(game, language, query, limit)
Search monsters

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**game** | **String** |  | [required] |
**language** | **String** |  | [required] |
**query** | **String** |  | [required] |
**limit** | Option<**i32**> |  |  |[default to 8]

### Return type

[**Vec<models::MappedEntityListEntry>**](MappedEntityListEntry.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## search_spells

> Vec<models::MappedEntityListEntry> search_spells(game, language, query, limit)
Search spells

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**game** | **String** |  | [required] |
**language** | **String** |  | [required] |
**query** | **String** |  | [required] |
**limit** | Option<**i32**> |  |  |[default to 8]

### Return type

[**Vec<models::MappedEntityListEntry>**](MappedEntityListEntry.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## search_subareas

> Vec<models::MappedEntityListEntry> search_subareas(game, language, query, limit)
Search subareas

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**game** | **String** |  | [required] |
**language** | **String** |  | [required] |
**query** | **String** |  | [required] |
**limit** | Option<**i32**> |  |  |[default to 8]

### Return type

[**Vec<models::MappedEntityListEntry>**](MappedEntityListEntry.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## search_super_areas

> Vec<models::MappedEntityListEntry> search_super_areas(game, language, query, limit)
Search super-areas

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**game** | **String** |  | [required] |
**language** | **String** |  | [required] |
**query** | **String** |  | [required] |
**limit** | Option<**i32**> |  |  |[default to 8]

### Return type

[**Vec<models::MappedEntityListEntry>**](MappedEntityListEntry.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

