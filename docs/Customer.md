# Customer Overview ✨

Customers on **Woodcore** are your end-users. They can be **individual** customers or **corporate** customers that make use of your product. The first point of entry in banking is gathering customer information, often referred to as the **Customer Information File (CIF)**.

<blockquote style="background-color: lightcyan; padding: 20px; border-left: 5px solid green; border-radius: 5px;"> 
<strong>👍<span style="color: green;">Classic Example</span></strong><br>
Think of <strong>Mark</strong> as an individual customer, Single signatory to an account.
</blockquote>

<blockquote style="background-color: floralwhite; padding: 20px; border-left: 5px solid sandybrown; border-radius: 5px;">
🚧 Customer can be created in a <strong>Pending</strong> or <strong>Active</strong> state
</blockquote>

In an attempt to create a customer for the first time, it is optional to create a deposit account for the customer on the go!. i.e., You can create a customer, a deposit account and block the deposit account from making transactions until KYC requirements are met.

<blockquote style="background-color: floralwhite; padding: 20px; border-left: 5px solid sandybrown; border-radius: 5px;"> 
🚧
Take note of the <code>clientType</code>. It is useful in specifying the kind of customer, either an <code>individual</code> or <code>corporate</code>customer.
</blockquote>

#### Note:
<ol>
<li> You can enter either: <code>firstname</code>, <code>middlename</code>, <code>lastname</code> - for an individual (<code>middlename</code> is optional) OR
<code>fullname</code> - for a business or corporate body (or person known by one name).</li>
<li>If address is enabled (<code>_isAddressEnabled=true</code>), then the customer's address can be created following specified parameters for the customer. To enable address on the WoodCore console, go to <i>Configuration</i> —> <i>Utilities</i> —> <i>Configuration</i> —> <i>Enable-Address</i>.</li>
</ol>



---

> ### Tier Level Configuration
>
>You can configure a client's **tierLevel** directly via the WoodCore console during customer creation. Alternatively, through the provided APIs.

---
