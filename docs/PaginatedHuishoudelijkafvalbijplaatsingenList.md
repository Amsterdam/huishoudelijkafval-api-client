# PaginatedHuishoudelijkafvalbijplaatsingenList


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page** | [**PaginatedHuishoudelijkafvaladresLoopafstandV2ListPage**](PaginatedHuishoudelijkafvaladresLoopafstandV2ListPage.md) |  | [optional] 
**links** | [**PaginatedHuishoudelijkafvaladresLoopafstandV2ListLinks**](PaginatedHuishoudelijkafvaladresLoopafstandV2ListLinks.md) |  | [optional] 
**embedded** | [**PaginatedHuishoudelijkafvalbijplaatsingenListEmbedded**](PaginatedHuishoudelijkafvalbijplaatsingenListEmbedded.md) |  | [optional] 

## Example

```python
from huishoudelijkafval_api_client.models.paginated_huishoudelijkafvalbijplaatsingen_list import PaginatedHuishoudelijkafvalbijplaatsingenList

# TODO update the JSON string below
json = "{}"
# create an instance of PaginatedHuishoudelijkafvalbijplaatsingenList from a JSON string
paginated_huishoudelijkafvalbijplaatsingen_list_instance = PaginatedHuishoudelijkafvalbijplaatsingenList.from_json(json)
# print the JSON string representation of the object
print(PaginatedHuishoudelijkafvalbijplaatsingenList.to_json())

# convert the object into a dict
paginated_huishoudelijkafvalbijplaatsingen_list_dict = paginated_huishoudelijkafvalbijplaatsingen_list_instance.to_dict()
# create an instance of PaginatedHuishoudelijkafvalbijplaatsingenList from a dict
paginated_huishoudelijkafvalbijplaatsingen_list_from_dict = PaginatedHuishoudelijkafvalbijplaatsingenList.from_dict(paginated_huishoudelijkafvalbijplaatsingen_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


