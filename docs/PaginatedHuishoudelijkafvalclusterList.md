# PaginatedHuishoudelijkafvalclusterList


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page** | [**PaginatedHuishoudelijkafvaladresLoopafstandV2ListPage**](PaginatedHuishoudelijkafvaladresLoopafstandV2ListPage.md) |  | [optional] 
**links** | [**PaginatedHuishoudelijkafvaladresLoopafstandV2ListLinks**](PaginatedHuishoudelijkafvaladresLoopafstandV2ListLinks.md) |  | [optional] 
**embedded** | [**PaginatedHuishoudelijkafvalclusterListEmbedded**](PaginatedHuishoudelijkafvalclusterListEmbedded.md) |  | [optional] 

## Example

```python
from huishoudelijkafval_api_client.models.paginated_huishoudelijkafvalcluster_list import PaginatedHuishoudelijkafvalclusterList

# TODO update the JSON string below
json = "{}"
# create an instance of PaginatedHuishoudelijkafvalclusterList from a JSON string
paginated_huishoudelijkafvalcluster_list_instance = PaginatedHuishoudelijkafvalclusterList.from_json(json)
# print the JSON string representation of the object
print(PaginatedHuishoudelijkafvalclusterList.to_json())

# convert the object into a dict
paginated_huishoudelijkafvalcluster_list_dict = paginated_huishoudelijkafvalcluster_list_instance.to_dict()
# create an instance of PaginatedHuishoudelijkafvalclusterList from a dict
paginated_huishoudelijkafvalcluster_list_from_dict = PaginatedHuishoudelijkafvalclusterList.from_dict(paginated_huishoudelijkafvalcluster_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


