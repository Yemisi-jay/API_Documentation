# Default Parameters

____
<blockquote style="background-color: floralwhite; padding: 20px; border-left: 5px solid brown; border-radius: 5px;"> 
 🚧 <strong style="color: #eb9950">Important </strong>🚦<br>
    The details on this page are critical. Please read carefully.
</blockquote>

There are specific keys and values that must be used as defaults in WoodCore's API request bodies or response queries. Below are the required attributes:

| **Attribute** | **Required** | **Comments**                                                                                            |
|---------------|--------------|---------------------------------------------------------------------------------------------------------|
| resourceId    | true         | This attribute acknowledges a `POST` request.                                                           |
| officeId      | true         | Offices represent the structure of MFIs. Use `GET /office` to verify the office you are operating from. |

---

<blockquote style="background-color: aliceblue; padding: 20px; border-left: 5px solid skyblue ; border-radius: 5px;">
📘 <strong style="color: #6ab0de;">Sample Date</strong> <br> 
Dates in WoodCore adhere to the format <code>dd/MMMM/yyyy.</code> Any other formats (e.g., <code>12/07/2023</code>, <code>16 dec 2023</code>) will not be accepted.  

A valid sample date on WoodCore appears as:  
<code>21 April 2021</code>,  
<code>08 December 2022</code>.
</blockquote>