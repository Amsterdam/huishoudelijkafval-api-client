# PaginatedHuishoudelijkafvalrolcontainerList


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page** | [**PaginatedHuishoudelijkafvaladresLoopafstandV2ListPage**](PaginatedHuishoudelijkafvaladresLoopafstandV2ListPage.md) |  | [optional] 
**links** | [**PaginatedHuishoudelijkafvaladresLoopafstandV2ListLinks**](PaginatedHuishoudelijkafvaladresLoopafstandV2ListLinks.md) |  | [optional] 
**embedded** | [**PaginatedHuishoudelijkafvalrolcontainerListEmbedded**](PaginatedHuishoudelijkafvalrolcontainerListEmbedded.md) |  | [optional] 

## Example

```python
from huishoudelijkafval_api_client.models.paginated_huishoudelijkafvalrolcontainer_list import PaginatedHuishoudelijkafvalrolcontainerList

# TODO update the JSON string below
json = "{}"
# create an instance of PaginatedHuishoudelijkafvalrolcontainerList from a JSON string
paginated_huishoudelijkafvalrolcontainer_list_instance = PaginatedHuishoudelijkafvalrolcontainerList.from_json(json)
# print the JSON string representation of the object
print(PaginatedHuishoudelijkafvalrolcontainerList.to_json())

# convert the object into a dict
paginated_huishoudelijkafvalrolcontainer_list_dict = paginated_huishoudelijkafvalrolcontainer_list_instance.to_dict()
# create an instance of PaginatedHuishoudelijkafvalrolcontainerList from a dict
paginated_huishoudelijkafvalrolcontainer_list_from_dict = PaginatedHuishoudelijkafvalrolcontainerList.from_dict(paginated_huishoudelijkafvalrolcontainer_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


