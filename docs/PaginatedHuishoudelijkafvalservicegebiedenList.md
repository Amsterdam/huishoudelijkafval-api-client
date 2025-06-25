# PaginatedHuishoudelijkafvalservicegebiedenList


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page** | [**PaginatedHuishoudelijkafvaladresLoopafstandV2ListPage**](PaginatedHuishoudelijkafvaladresLoopafstandV2ListPage.md) |  | [optional] 
**links** | [**PaginatedHuishoudelijkafvaladresLoopafstandV2ListLinks**](PaginatedHuishoudelijkafvaladresLoopafstandV2ListLinks.md) |  | [optional] 
**embedded** | [**PaginatedHuishoudelijkafvalservicegebiedenListEmbedded**](PaginatedHuishoudelijkafvalservicegebiedenListEmbedded.md) |  | [optional] 

## Example

```python
from huishoudelijkafval_api_client.models.paginated_huishoudelijkafvalservicegebieden_list import PaginatedHuishoudelijkafvalservicegebiedenList

# TODO update the JSON string below
json = "{}"
# create an instance of PaginatedHuishoudelijkafvalservicegebiedenList from a JSON string
paginated_huishoudelijkafvalservicegebieden_list_instance = PaginatedHuishoudelijkafvalservicegebiedenList.from_json(json)
# print the JSON string representation of the object
print(PaginatedHuishoudelijkafvalservicegebiedenList.to_json())

# convert the object into a dict
paginated_huishoudelijkafvalservicegebieden_list_dict = paginated_huishoudelijkafvalservicegebieden_list_instance.to_dict()
# create an instance of PaginatedHuishoudelijkafvalservicegebiedenList from a dict
paginated_huishoudelijkafvalservicegebieden_list_from_dict = PaginatedHuishoudelijkafvalservicegebiedenList.from_dict(paginated_huishoudelijkafvalservicegebieden_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


