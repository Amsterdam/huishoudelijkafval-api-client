# PaginatedHuishoudelijkafvalservicegebiedenLocatieList


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page** | [**PaginatedHuishoudelijkafvaladresLoopafstandV2ListPage**](PaginatedHuishoudelijkafvaladresLoopafstandV2ListPage.md) |  | [optional] 
**links** | [**PaginatedHuishoudelijkafvaladresLoopafstandV2ListLinks**](PaginatedHuishoudelijkafvaladresLoopafstandV2ListLinks.md) |  | [optional] 
**embedded** | [**PaginatedHuishoudelijkafvalservicegebiedenLocatieListEmbedded**](PaginatedHuishoudelijkafvalservicegebiedenLocatieListEmbedded.md) |  | [optional] 

## Example

```python
from huishoudelijkafval_api_client.models.paginated_huishoudelijkafvalservicegebieden_locatie_list import PaginatedHuishoudelijkafvalservicegebiedenLocatieList

# TODO update the JSON string below
json = "{}"
# create an instance of PaginatedHuishoudelijkafvalservicegebiedenLocatieList from a JSON string
paginated_huishoudelijkafvalservicegebieden_locatie_list_instance = PaginatedHuishoudelijkafvalservicegebiedenLocatieList.from_json(json)
# print the JSON string representation of the object
print(PaginatedHuishoudelijkafvalservicegebiedenLocatieList.to_json())

# convert the object into a dict
paginated_huishoudelijkafvalservicegebieden_locatie_list_dict = paginated_huishoudelijkafvalservicegebieden_locatie_list_instance.to_dict()
# create an instance of PaginatedHuishoudelijkafvalservicegebiedenLocatieList from a dict
paginated_huishoudelijkafvalservicegebieden_locatie_list_from_dict = PaginatedHuishoudelijkafvalservicegebiedenLocatieList.from_dict(paginated_huishoudelijkafvalservicegebieden_locatie_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


