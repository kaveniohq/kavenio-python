# SelectLinkedInOrganizationRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**account_id** | **str** |  | 
**profile_id** | **str** |  | 
**organization_urn** | **str** |  | 
**display_name** | **str** |  | [optional] 

## Example

```python
from kavenio.models.select_linked_in_organization_request import SelectLinkedInOrganizationRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SelectLinkedInOrganizationRequest from a JSON string
select_linked_in_organization_request_instance = SelectLinkedInOrganizationRequest.from_json(json)
# print the JSON string representation of the object
print(SelectLinkedInOrganizationRequest.to_json())

# convert the object into a dict
select_linked_in_organization_request_dict = select_linked_in_organization_request_instance.to_dict()
# create an instance of SelectLinkedInOrganizationRequest from a dict
select_linked_in_organization_request_from_dict = SelectLinkedInOrganizationRequest.from_dict(select_linked_in_organization_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


