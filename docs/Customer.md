# Customer Overview ✨

Customers on **Woodcore** are your end-users. They can be **individual** customers or **corporate** customers that make use of your product. The first point of entry in banking is gathering customer information, often referred to as the **Customer Information File (CIF)**.

>  **Classic Example:**
> Think of Mark as an individual customer, Single signatory to an account.

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

> **Classic Example:**  
> Think of *Mark* as an individual customer, acting as the sole signatory to an account.

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
  - **Note:**  
    You can create a customer along with a deposit account and block the account from making transactions until the KYC (Know Your Customer) requirements are met.

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
> - You can configure a client's **tierLevel**:
>  - Directly via the WoodCore console during customer creation.
>  - Alternatively, through the provided APIs.

---
