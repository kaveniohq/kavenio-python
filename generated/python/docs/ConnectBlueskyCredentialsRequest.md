# ConnectBlueskyCredentialsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**profile_id** | **str** |  | 
**identifier** | **str** |  | 
**app_password** | **str** |  | 
**pds_url** | **str** |  | [optional] 

## Example

```python
from kavenio.models.connect_bluesky_credentials_request import ConnectBlueskyCredentialsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ConnectBlueskyCredentialsRequest from a JSON string
connect_bluesky_credentials_request_instance = ConnectBlueskyCredentialsRequest.from_json(json)
# print the JSON string representation of the object
print(ConnectBlueskyCredentialsRequest.to_json())

# convert the object into a dict
connect_bluesky_credentials_request_dict = connect_bluesky_credentials_request_instance.to_dict()
# create an instance of ConnectBlueskyCredentialsRequest from a dict
connect_bluesky_credentials_request_from_dict = ConnectBlueskyCredentialsRequest.from_dict(connect_bluesky_credentials_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


