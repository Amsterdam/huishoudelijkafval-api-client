# PaginatedHuishoudelijkafvalclusterfractieList


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page** | [**PaginatedHuishoudelijkafvaladresLoopafstandV2ListPage**](PaginatedHuishoudelijkafvaladresLoopafstandV2ListPage.md) |  | [optional] 
**links** | [**PaginatedHuishoudelijkafvaladresLoopafstandV2ListLinks**](PaginatedHuishoudelijkafvaladresLoopafstandV2ListLinks.md) |  | [optional] 
**embedded** | [**PaginatedHuishoudelijkafvalclusterfractieListEmbedded**](PaginatedHuishoudelijkafvalclusterfractieListEmbedded.md) |  | [optional] 

## Example

```python
from huishoudelijkafval_api_client.models.paginated_huishoudelijkafvalclusterfractie_list import PaginatedHuishoudelijkafvalclusterfractieList

# TODO update the JSON string below
json = "{}"
# create an instance of PaginatedHuishoudelijkafvalclusterfractieList from a JSON string
paginated_huishoudelijkafvalclusterfractie_list_instance = PaginatedHuishoudelijkafvalclusterfractieList.from_json(json)
# print the JSON string representation of the object
print(PaginatedHuishoudelijkafvalclusterfractieList.to_json())

# convert the object into a dict
paginated_huishoudelijkafvalclusterfractie_list_dict = paginated_huishoudelijkafvalclusterfractie_list_instance.to_dict()
# create an instance of PaginatedHuishoudelijkafvalclusterfractieList from a dict
paginated_huishoudelijkafvalclusterfractie_list_from_dict = PaginatedHuishoudelijkafvalclusterfractieList.from_dict(paginated_huishoudelijkafvalclusterfractie_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


