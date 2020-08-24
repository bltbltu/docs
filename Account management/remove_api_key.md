**URL** 

- `/private/remove_api_key`

Removes api key



*This is a private method; it can only be used after authentication.*

**Parameters** 

| Parameter | Required | Type    | Enum | Description |
| :-------- | :------- | :------ | ---- | ----------- |
| id        | true     | integer |      | Id of key   |



**Response**

| **Name** | **Type** | **Description**                                     |
| :------- | :------- | --------------------------------------------------- |
| id       | string   | The id that was sent in the request                 |
| jsonrpc  | string   | The JSON-RPC version (2.0)                          |
| usIn     | integer  | The timestamp when the requests was received (microseconds since the Unix epoch)                                           |
| usOut    | integer  | The timestamp when the response was sent (microseconds since the Unix epoch)                                          |
| usDiff   | integer  | The number of microseconds that was spent handling the request                                                |
| result   | string   | Result of method execution. `ok` in case of success |

example:

```json
{
	"id": "11",
	"jsonrpc": "2.0",
	"usIn": 1597127976248,
	"usOut": 1597127976286,
	"usDiff": 38,
	"result": [{
		"timestamp": "1596837665180",
		"max_scope": "account:read_write,block_trade:read_write,trade:read_write,wallet:read_write",
		"id": 124,
		"enabled": true,
		"client_secret": "a07d4394b4ed7b8f7567432c",
		"client_id": "b2b76b28",
		"name": "test",
		"ip_whitelist": [],
		"default": true
	}]
}
```
