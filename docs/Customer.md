# Customer Overview ✨

Customers on **Woodcore** are your end-users. They can be **individual** customers or **corporate** customers that make use of your product. The first point of entry in banking is gathering customer information, often referred to as the **Customer Information File (CIF)**.

<blockquote style="background-color: lightcyan; padding: 20px; border-left: 5px solid green; border-radius: 5px;"> 
<strong>👍<span style="color: green;">Classic Example</span></strong><br>
Think of <strong>Mark</strong> as an individual customer, Single signatory to an account.
</blockquote>

<blockquote style="background-color: floralwhite; padding: 20px; border-left: 5px solid sandybrown; border-radius: 5px;">
🚧 Customer can be created in a <bold>Pending</bold> or <bold>Active</bold> state
</blockquote>

##### Customer Types

- **Individual Customers**  
  - Represent a single signatory, e.g., Mark.
  - Use the following fields:
    - `firstname`
    - `middlename` (optional)
    - `lastname`

- **Corporate Customers**  
  - Represent a business or any entity known by a single name.
  - Use the following field:
    - `fullname`

<blockquote style="background-color: lightcyan; padding: 20px; border-left: 5px solid green; border-radius: 5px;"> 
<strong>👍<span style="color: green;">Classic Example</span></strong><br>
Think of <strong>Mark</strong> as an individual customer, acting as the sole signatory to an account.
</blockquote>

---

### Customer Status

- **Pending:**  
  Customers can be created with a pending status.

- **Active:**  
  Customers can also be created directly in an active state.

---

### Account Creation Workflow

- **Optional Deposit Account Creation:**  
  When creating a customer for the first time, you have the option to create a deposit account simultaneously.
<blockquote style="background-color: gainsboro; padding: 20px; border-left: 5px solid brown; border-radius: 5px;"> 
📌<strong>Note</strong><br>  
    You can create a customer along with a deposit account and block the account from making transactions until the KYC (Know Your Customer) requirements are met.
</blockquote>
---

### Client Type Specification

- **clientType Field:**  
  This field is used to specify the kind of customer:
  - `individual`
  - `corporate`

---

### Address Configuration

- **Enabling Address Information:**  
  If address information is enabled (`_isAddressEnabled=true`), the customer's address can be captured following the specified parameters.
  
  - **To Enable Address on the WoodCore Console:**
    1. Navigate to **Configuration**
    2. Select **Utilities**
    3. Go to **Configuration**
    4. Choose **Enable-Address**

---

> ### Tier Level Configuration
>
>You can configure a client's **tierLevel** directly via the WoodCore console during customer creation. Alternatively, through the provided APIs.

---
