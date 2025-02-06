# Reference

## API Design 🔥

The **WoodCore API** is organized around **REST**. It features:  
- Predictable resource-oriented URLs  
- Form-encoded request bodies  
- JSON-encoded responses  
- Standard HTTP response codes, authentication, and verbs  

You can use the **WoodCore API** for free in **Sandbox mode**.  
- Sandbox mode does not affect your data in **Production mode** and does not interact with production financial services.  
- It provides a testing environment only.  

**Production mode** offers:  
- Full, unlimited access to every feature in your selected plan  
- Processing of live requests  

<blockquote style="background-color:  cornsilk; color: #721c24; padding: 10px; border-left: 5px solid #f5c6cb; border-radius: 5px;">🚧 **Important:** 
The API key you use for authentication determines whether your request runs in Sandbox or **Production mode**.  
API keys for both environments are available upon request at [hello@woodcoreapp.com](mailto:hello@woodcoreapp.com).
</blockquote>

<blockquote style="background-color: powderblue; color: #721c24; padding: 10px; border-left: 5px solid skyblue ; border-radius: 5px;">📘 **API Key Format:**  
Sandbox keys:** `wc_test_{{api_key}}`  
Production/Live keys:** `wc_live_{{api_key}}`  
</blockquote>

---

## API Protocol

The **WoodCore API** follows the **REST** standard and adheres to the **RFC 2616** protocol.  
- Uses `GET` and `POST` requests  
- Returns **HTTP response codes** to indicate status and errors  

### **Request & Response Format**
- All responses are in **JSON format**  
- All requests **must** include:  
  - `Content-Type: application/json` header  
  - A valid JSON body (when required)  

### **Security**
The API is served over **HTTPS TLS v1.2** for **data privacy**.  

> ❗ **Security Notice:**  
> The API **only supports** secure communications over **HTTPS TLS v1.2**.  
> Connections using HTTP or **TLS 1.1 and below** are **not supported** and will be rejected.  

