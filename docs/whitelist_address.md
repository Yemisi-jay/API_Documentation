# Whitelist an IP Address

<div style="background-color: #0ea5e9; font-size: 0.9em; color: white; display: inline-block; padding: 2px 5px; border-radius: 7px;">
  POST
</div> 
<span style="font-size: 0.9em; color: #333; margin-left: 10px;">
  <a href="https://spark.test.woodcore.co/api/v2/gateway/apiKeys/ipwhitelist" style="text-decoration: none; color: #333;">https://spark.test.woodcore.co/api/v2/gateway/apiKeys/ipwhitelist</a>
</span>

This endpoint is responsible for whitelisting an IP address, which is to be attached to a particular API KEY.

<div style="background-color: #e5f7ff; border-left: 4px solid #0ea5e9; padding: 10px; margin: 10px 0; border-radius: 5px;">
  <strong style="color: #0284c7;">Note:</strong>
  Please keep in mind that you can only whitelist a single IP address for each API KEY with this endpoint. However, you can modify the IP address linked to the API KEY as needed using this endpoint.
</div>

<div style="background-color: #e5f7ff; border-left: 4px solid #0ea5e9; padding: 10px; margin: 10px 0; border-radius: 5px;">
  <strong style="color: #0284c7;">Production URL:</strong>
  It is important to also note that the production URL for this endpoint is:
  <br>
  <a href="https://api.woodcoreapp.com/api/v2/gateway/apiKeys/ipwhitelist" style="color: #333;">https://api.woodcoreapp.com/api/v2/gateway/apiKeys/ipwhitelist</a>
</div>

---

# Whitelist IP Address API

## **Body Parameters**
| Parameter | Type   | Required | Default  | Description |
|-----------|--------|----------|----------|-------------|
| `ips`     | string | ✅ Yes   | 1.2.3.1 | The IP address to be whitelisted for the API key. |

> **If the request is successful, an OTP will be sent to the user's email for verification.**

## **Responses**
| Status Code | Description                      |
|-------------|----------------------------------|
| ✅ **200**  | OTP sent successfully.           |
| ❌ **400**  | Invalid IP format.               |



### Code Examples

??? example "python"
    === "code"
```python
# Install the requests library
python -m pip install requests

import requests

url = "https://spark.test.woodcore.co/api/v2/gateway/apiKeys/ipwhitelist"

payload = { "ips": "1.2.3.1" }
headers = {
    "accept": "application/json",
    "content-type": "application/json",
}

response = requests.post(url, json=payload, headers=headers)

print(response.text)
```