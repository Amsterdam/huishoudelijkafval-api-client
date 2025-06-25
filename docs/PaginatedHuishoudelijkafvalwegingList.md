# PaginatedHuishoudelijkafvalwegingList


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page** | [**PaginatedHuishoudelijkafvaladresLoopafstandV2ListPage**](PaginatedHuishoudelijkafvaladresLoopafstandV2ListPage.md) |  | [optional] 
**links** | [**PaginatedHuishoudelijkafvaladresLoopafstandV2ListLinks**](PaginatedHuishoudelijkafvaladresLoopafstandV2ListLinks.md) |  | [optional] 
**embedded** | [**PaginatedHuishoudelijkafvalwegingListEmbedded**](PaginatedHuishoudelijkafvalwegingListEmbedded.md) |  | [optional] 

## Example

```python
from huishoudelijkafval_api_client.models.paginated_huishoudelijkafvalweging_list import PaginatedHuishoudelijkafvalwegingList

# TODO update the JSON string below
json = "{}"
# create an instance of PaginatedHuishoudelijkafvalwegingList from a JSON string
paginated_huishoudelijkafvalweging_list_instance = PaginatedHuishoudelijkafvalwegingList.from_json(json)
# print the JSON string representation of the object
print(PaginatedHuishoudelijkafvalwegingList.to_json())

# convert the object into a dict
paginated_huishoudelijkafvalweging_list_dict = paginated_huishoudelijkafvalweging_list_instance.to_dict()
# create an instance of PaginatedHuishoudelijkafvalwegingList from a dict
paginated_huishoudelijkafvalweging_list_from_dict = PaginatedHuishoudelijkafvalwegingList.from_dict(paginated_huishoudelijkafvalweging_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


