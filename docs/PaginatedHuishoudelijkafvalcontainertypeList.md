# PaginatedHuishoudelijkafvalcontainertypeList


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page** | [**PaginatedHuishoudelijkafvaladresLoopafstandV2ListPage**](PaginatedHuishoudelijkafvaladresLoopafstandV2ListPage.md) |  | [optional] 
**links** | [**PaginatedHuishoudelijkafvaladresLoopafstandV2ListLinks**](PaginatedHuishoudelijkafvaladresLoopafstandV2ListLinks.md) |  | [optional] 
**embedded** | [**PaginatedHuishoudelijkafvalcontainertypeListEmbedded**](PaginatedHuishoudelijkafvalcontainertypeListEmbedded.md) |  | [optional] 

## Example

```python
from huishoudelijkafval_api_client.models.paginated_huishoudelijkafvalcontainertype_list import PaginatedHuishoudelijkafvalcontainertypeList

# TODO update the JSON string below
json = "{}"
# create an instance of PaginatedHuishoudelijkafvalcontainertypeList from a JSON string
paginated_huishoudelijkafvalcontainertype_list_instance = PaginatedHuishoudelijkafvalcontainertypeList.from_json(json)
# print the JSON string representation of the object
print(PaginatedHuishoudelijkafvalcontainertypeList.to_json())

# convert the object into a dict
paginated_huishoudelijkafvalcontainertype_list_dict = paginated_huishoudelijkafvalcontainertype_list_instance.to_dict()
# create an instance of PaginatedHuishoudelijkafvalcontainertypeList from a dict
paginated_huishoudelijkafvalcontainertype_list_from_dict = PaginatedHuishoudelijkafvalcontainertypeList.from_dict(paginated_huishoudelijkafvalcontainertype_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


