# PaginatedHuishoudelijkafvalticketList


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page** | [**PaginatedHuishoudelijkafvaladresLoopafstandV2ListPage**](PaginatedHuishoudelijkafvaladresLoopafstandV2ListPage.md) |  | [optional] 
**links** | [**PaginatedHuishoudelijkafvaladresLoopafstandV2ListLinks**](PaginatedHuishoudelijkafvaladresLoopafstandV2ListLinks.md) |  | [optional] 
**embedded** | [**PaginatedHuishoudelijkafvalticketListEmbedded**](PaginatedHuishoudelijkafvalticketListEmbedded.md) |  | [optional] 

## Example

```python
from huishoudelijkafval_api_client.models.paginated_huishoudelijkafvalticket_list import PaginatedHuishoudelijkafvalticketList

# TODO update the JSON string below
json = "{}"
# create an instance of PaginatedHuishoudelijkafvalticketList from a JSON string
paginated_huishoudelijkafvalticket_list_instance = PaginatedHuishoudelijkafvalticketList.from_json(json)
# print the JSON string representation of the object
print(PaginatedHuishoudelijkafvalticketList.to_json())

# convert the object into a dict
paginated_huishoudelijkafvalticket_list_dict = paginated_huishoudelijkafvalticket_list_instance.to_dict()
# create an instance of PaginatedHuishoudelijkafvalticketList from a dict
paginated_huishoudelijkafvalticket_list_from_dict = PaginatedHuishoudelijkafvalticketList.from_dict(paginated_huishoudelijkafvalticket_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


