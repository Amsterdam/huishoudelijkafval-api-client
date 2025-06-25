# PaginatedHuishoudelijkafvalcontainerList


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page** | [**PaginatedHuishoudelijkafvaladresLoopafstandV2ListPage**](PaginatedHuishoudelijkafvaladresLoopafstandV2ListPage.md) |  | [optional] 
**links** | [**PaginatedHuishoudelijkafvaladresLoopafstandV2ListLinks**](PaginatedHuishoudelijkafvaladresLoopafstandV2ListLinks.md) |  | [optional] 
**embedded** | [**PaginatedHuishoudelijkafvalcontainerListEmbedded**](PaginatedHuishoudelijkafvalcontainerListEmbedded.md) |  | [optional] 

## Example

```python
from huishoudelijkafval_api_client.models.paginated_huishoudelijkafvalcontainer_list import PaginatedHuishoudelijkafvalcontainerList

# TODO update the JSON string below
json = "{}"
# create an instance of PaginatedHuishoudelijkafvalcontainerList from a JSON string
paginated_huishoudelijkafvalcontainer_list_instance = PaginatedHuishoudelijkafvalcontainerList.from_json(json)
# print the JSON string representation of the object
print(PaginatedHuishoudelijkafvalcontainerList.to_json())

# convert the object into a dict
paginated_huishoudelijkafvalcontainer_list_dict = paginated_huishoudelijkafvalcontainer_list_instance.to_dict()
# create an instance of PaginatedHuishoudelijkafvalcontainerList from a dict
paginated_huishoudelijkafvalcontainer_list_from_dict = PaginatedHuishoudelijkafvalcontainerList.from_dict(paginated_huishoudelijkafvalcontainer_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


