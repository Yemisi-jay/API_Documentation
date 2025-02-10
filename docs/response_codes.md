# Response Codes

----

### HTTP Status Codes  

Below is a detailed explanation of the response codes used by the WoodCore client and server. Familiarity with these codes will help you better understand API behavior.  

| **Code** | **Response Type**       | **Description**                                                                                                                                     |
|----------|-------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------|
| **200**  | OK                      | The request was successful, and everything worked as expected.                                                                                      |
| **202**  | Data Extraction Pending | The data extraction process is in progress. At this point, you should switch to asynchronous handling using webhook events.                         |
| **204**  | No Data Extracted       | The account does not have data for the requested reporting period. <br> **Note**: Filters resulting in no data for extracted periods will return an empty array along with a 200 response code. |
| **400**  | Bad Request             | The request was invalid, often due to missing or improperly formatted parameters.                                                                   |
| **401**  | Unauthorized            | The request lacked valid API keys or access tokens.                                                                                                 |
| **403**  | Forbidden               | The API key does not have permission to perform this action or is restricted based on the current billing plan.                                     |
| **404**  | Resource Not Found      | The requested resource could not be found.                                                                                                          |
| **409**  | Conflict                | The request conflicts with another request.                                                                                                         |
| **429**  | Too much requests       | Too many requests hit the API too quickly. We recommend an exponential backoff of your requests.                                                    |
| **500**  | Server Error            | An unexpected error and could not process your request.                                                                                             |
| **502**  | Bad Gateway             | Invalid response received from serer.                                                                                                               |
| **503**  | Service Unavailable     | WoodCore is temporarily offline for maintenance.                                                                                                    |
| **504**  | Service Timeout         | The request timed out from the server.                                                                                                              |

This guide ensures a clear understanding of the server's response, aiding in effective debugging and implementation of API requests.
