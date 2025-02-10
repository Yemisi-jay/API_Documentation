# Approve Whitelisted IP

<div style="background-color: #0ea5e9; font-size: 0.9em; color: white; display: inline-block; padding: 2px 5px; border-radius: 7px;">
  POST
</div> 
<span style="font-size: 0.9em; color: #333; margin-left: 10px;">
  <a href="https://spark.test.woodcore.co/api/v2/gateway/apiKeys/ipwhitelist/approve/{otp}" style="text-decoration: none; color: #333;">https://spark.test.woodcore.co/api/v2/gateway/apiKeys/ipwhitelist/approve/{otp}</a>
</span>


This endpoint approves a whitelisted IP address with the use of an OTP in the path sent to the user's email address as an extra layer of security.

---
<div style="background-color: #e5f7ff; border-left: 4px solid #0ea5e9; padding: 10px; margin: 10px 0; border-radius: 5px;">
  <strong style="color: #0284c7;"> 📝 Note</strong><br><br>



    For every additional IP address that is added after an initial addition, the value of the stored IP changes/updates instead of adding another IP Address, which increases the total number of IPs associated with an API KEY.<br><br>

    <i>This implies that <strong>only one IP address is associated with a Key at any point in time.</i></strong>
</div>
---

<div style="background-color: #e5f7ff; border-left: 4px solid #0ea5e9; padding: 10px; margin: 10px 0; border-radius: 5px;">
  <strong style="color: #0284c7;"> 🌐 Production URL</strong><br><br>


    The production URL for this endpoint is:<br><br>
    <a href="https://api.woodcoreapp.com/api/v2/gateway/apiKeys/ipwhitelist/approve/">https://api.woodcoreapp.com/api/v2/gateway/apiKeys/ipwhitelist/approve/</a>
</div>


---

### **Body Parameters**
| Parameter | Type   | Required | Default     | Description                                   |
|-----------|--------|----------|-------------|-----------------------------------------------|
| `ips`     | string | ✅ Yes   | 7edllzm84ut | The IP address to be approved whitelisted IP. |

----

### **Responses**
| Status Code | Description                      |
|-------------|----------------------------------|
| ✅ **200**  | OTP sent successfully.           |
| ❌ **400**  | Invalid IP format.               |

----

#### 🔗 Example Request (Python)

```python
# Install requests library if not installed
python -m pip install requests

import requests

url = "https://spark.test.woodcore.co/api/v2/gateway/apiKeys/ipwhitelist/approve/{otp}"
headers = {"accept": "application/json"}

response = requests.post(url, headers=headers)

print(response.text)
```