# ReferentiekalenderdatumLink

The identifier of the relationship to datum.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**href** | **str** |  | [readonly] 
**title** | **str** |  | 
**id** | **int** | Sleutelveld. Bij niveaucode dag is dit in feite de juliaanse dag. Zo kan bijvoorbeeld het verschil tussen twee datums bepaald worden door het verschil tussen de ID waarden van de datums te berekenen. De id waarden zijn zo geconstrueerd dat dit altijd kan ongeacht de waarde van niveaucode. Dus als b.v. niveaucode is &#39;Week&#39; dan bevat een verschil in id waarden het aantal weken tussen de twee week records. | 

## Example

```python
from huishoudelijkafval_api_client.models.referentiekalenderdatum_link import ReferentiekalenderdatumLink

# TODO update the JSON string below
json = "{}"
# create an instance of ReferentiekalenderdatumLink from a JSON string
referentiekalenderdatum_link_instance = ReferentiekalenderdatumLink.from_json(json)
# print the JSON string representation of the object
print(ReferentiekalenderdatumLink.to_json())

# convert the object into a dict
referentiekalenderdatum_link_dict = referentiekalenderdatum_link_instance.to_dict()
# create an instance of ReferentiekalenderdatumLink from a dict
referentiekalenderdatum_link_from_dict = ReferentiekalenderdatumLink.from_dict(referentiekalenderdatum_link_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


