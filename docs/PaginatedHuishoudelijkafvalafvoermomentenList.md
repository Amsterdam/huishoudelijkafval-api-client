# PaginatedHuishoudelijkafvalafvoermomentenList


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page** | [**PaginatedHuishoudelijkafvaladresLoopafstandV2ListPage**](PaginatedHuishoudelijkafvaladresLoopafstandV2ListPage.md) |  | [optional] 
**links** | [**PaginatedHuishoudelijkafvaladresLoopafstandV2ListLinks**](PaginatedHuishoudelijkafvaladresLoopafstandV2ListLinks.md) |  | [optional] 
**embedded** | [**PaginatedHuishoudelijkafvalafvoermomentenListEmbedded**](PaginatedHuishoudelijkafvalafvoermomentenListEmbedded.md) |  | [optional] 

## Example

```python
from huishoudelijkafval_api_client.models.paginated_huishoudelijkafvalafvoermomenten_list import PaginatedHuishoudelijkafvalafvoermomentenList

# TODO update the JSON string below
json = "{}"
# create an instance of PaginatedHuishoudelijkafvalafvoermomentenList from a JSON string
paginated_huishoudelijkafvalafvoermomenten_list_instance = PaginatedHuishoudelijkafvalafvoermomentenList.from_json(json)
# print the JSON string representation of the object
print(PaginatedHuishoudelijkafvalafvoermomentenList.to_json())

# convert the object into a dict
paginated_huishoudelijkafvalafvoermomenten_list_dict = paginated_huishoudelijkafvalafvoermomenten_list_instance.to_dict()
# create an instance of PaginatedHuishoudelijkafvalafvoermomentenList from a dict
paginated_huishoudelijkafvalafvoermomenten_list_from_dict = PaginatedHuishoudelijkafvalafvoermomentenList.from_dict(paginated_huishoudelijkafvalafvoermomenten_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


