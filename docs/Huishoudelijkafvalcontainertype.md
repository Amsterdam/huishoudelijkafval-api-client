# Huishoudelijkafvalcontainertype

containertype

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**HuishoudelijkafvaldefaultContainertypeLinks**](HuishoudelijkafvaldefaultContainertypeLinks.md) |  | 
**id** | **str** | Unieke aanduiding objecttype | 
**naam** | **str** | Naam van het containertype | [optional] 
**volume_m3** | **float** | Het volume (m3) aan afval wat de container kan bevatten | [optional] 
**gewicht_kg** | **int** | Het volume (m3) aan afval wat de container kan bevatten | [optional] 
**wijzigingsdatum_dp** | **datetime** | Datum waarop het object is gewijzigd | [optional] 
**verwijderd_dp** | **bool** | Indicatie of het object verwijderd is bij de bronhouder | [optional] 
**containertype_artikelcode** | **str** | Artikelcodevan het het containertype. | [optional] 
**containertype_hijskraantype_naam** | **str** | Naam van het type hijskraantype. | [optional] 
**containertype_hijskraan_opmerking** | **str** | Opmerking over het hijskraantype | [optional] 
**containertype_container_type** | **str** | Het type van de container type | [optional] 
**containertype_compressie_container_ind** | **bool** | Indicatie voor aanwezigheid van compressie instrument. | [optional] 
**containertype_compressiefactor** | **str** | De compressiefactor van compressie instrument | [optional] 

## Example

```python
from huishoudelijkafval_api_client.models.huishoudelijkafvalcontainertype import Huishoudelijkafvalcontainertype

# TODO update the JSON string below
json = "{}"
# create an instance of Huishoudelijkafvalcontainertype from a JSON string
huishoudelijkafvalcontainertype_instance = Huishoudelijkafvalcontainertype.from_json(json)
# print the JSON string representation of the object
print(Huishoudelijkafvalcontainertype.to_json())

# convert the object into a dict
huishoudelijkafvalcontainertype_dict = huishoudelijkafvalcontainertype_instance.to_dict()
# create an instance of Huishoudelijkafvalcontainertype from a dict
huishoudelijkafvalcontainertype_from_dict = Huishoudelijkafvalcontainertype.from_dict(huishoudelijkafvalcontainertype_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


