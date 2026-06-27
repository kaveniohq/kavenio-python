# ConnectTelegramCredentialsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**profile_id** | **str** |  | 
**bot_token** | **str** |  | 
**chat_id** | **str** |  | [optional] 
**display_name** | **str** |  | [optional] 
**api_base_url** | **str** |  | [optional] 

## Example

```python
from kavenio.models.connect_telegram_credentials_request import ConnectTelegramCredentialsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ConnectTelegramCredentialsRequest from a JSON string
connect_telegram_credentials_request_instance = ConnectTelegramCredentialsRequest.from_json(json)
# print the JSON string representation of the object
print(ConnectTelegramCredentialsRequest.to_json())

# convert the object into a dict
connect_telegram_credentials_request_dict = connect_telegram_credentials_request_instance.to_dict()
# create an instance of ConnectTelegramCredentialsRequest from a dict
connect_telegram_credentials_request_from_dict = ConnectTelegramCredentialsRequest.from_dict(connect_telegram_credentials_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


