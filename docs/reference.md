# Reference

## API Design 🔥

The **WoodCore API** is organized around [REST](https://en.wikipedia.org/wiki/REST). Our API has predictable resource-oriented URLs, accepts form-encoded request bodies, produces JSON-encoded reponses, and adheres to standard HTTP response codes, authentication, and verbs.

You can use the **WoodCore API** for free in **Sandbox** mode. This has no effect on your data in Production mode, nor does it interact with any production instance from the financial service offerings. It is a test-only environment.

**Production mode** offers: Full, unlimited access to every feature in your selected plan and begins processing live requests when in use 

<blockquote style="background-color:  cornsilk; padding: 10px; border-left: 5px solid #f5c6cb; border-radius: 5px;">
🚧 Important: 
The <strong>API</strong> key you use for authentication determines whether your request runs in <strong>Sandbox</strong> or <strong>Production mode</strong>.  
API keys for Sandbox and Production environments are available upon request at <a href="mailto:hello@woodcoreapp.com">hello@woodcoreapp.com.</a>
</blockquote>

<blockquote style="background-color: aliceblue; padding: 20px; border-left: 5px solid skyblue ; border-radius: 5px;">
📘 API Key Format: <br>
<strong>Sandbox keys</strong>, starts with <code>wc_test_{{api_key}}</code><br>
<strong>Production/Live keys</strong>, starts with <code>wc_live_{{api_key}}</code>  
</blockquote>

---

## API Protocol

The WoodCore API adheres to the **REST** standard making use of HTTP techniques outlined by the [RFC 2616](https://datatracker.ietf.org/doc/html/rfc2616) protocol. it uses `GET` and `POST` requests, returns HTTP [response codes](https://www.w3.org/Protocols/rfc2616/rfc2616-sec10.html) indicating status and errors.

### **Request & Response Format**
- All responses are in [JSON](https://www.json.org/json-en.html) format 
- All requests **must** include: `Content-Type: application/json` header and a valid JSON body (when required)  

### **Security**
The WoodCore API is served over **HTTPS TLS v1.2** for **data privacy**; HTTP or HTTPS with TLS equal 1.1 and below are not supported. 

<blockquote style="background-color: floralwhite; padding: 20px; border-left: 5px solid brown; border-radius: 5px;"> 
❗ Security Notice: 
The <strong>API</strong> only supports secure communications over <strong>HTTPS TLS v1.2</strong> to ensure data privacy.  
Connections using <strong>HTTP</strong> or <strong>HTTPS</strong> with <strong>TLS</strong> under <strong>v1.2</strong> are not supported and will be rejected.  
</blockquote>
