## Liquidity in Finance Terms

Liquidity refers to a company’s ability to meet its **short-term cash obligations** using available cash or cash-equivalent assets.

### Common Liquidity Items
- Cash in hand 
- Bank balances 
- Short-term investments 
- Incoming customer payments 
- Outgoing vendor payments 

📌 **Key Point:** 
Liquidity focuses on **cash movement and timing**, not on profit or accounting entries.

---

## Liquidity in SAP (Very Important)

In SAP systems such as **SAP Analytics Cloud (SAC) Cash Flow Planning** and **SAP S/4HANA / BW**, liquidity is tracked using a dedicated concept called **Liquidity Items**.

### 🔹 Liquidity Item
A **Liquidity Item** represents a specific **type of cash inflow or cash outflow**. 
It explains **why cash is increasing or decreasing**.

### Examples of Liquidity Items
- Customer Receipts 
- Vendor Payments 
- Payroll 
- Tax Payments 
- Loan Repayment 
- Interest Income 

👉 Liquidity Items help classify and analyze cash movements in **cash flow planning and reporting**. 

## Liquidity in the Architecture Diagram

In the shared SAP Cash Flow Planning architecture:

- **Liquidity Items** are used as a **dimension**
- Liquidity master data is sourced from **SAP BW**
- They are used to classify:
  - Cash inflows
  - Cash outflows
- Liquidity Items are used extensively in the **Cash Flow Planning Model**

### Example Mapping

GL Account → Liquidity Item → Cash Flow Category

This mapping helps convert accounting data into meaningful **cash flow insights**.

---

## Real-Time Example (Easy to Remember)

### Personal Cash Flow Example
- Salary credited on 1st → **Cash inflow**
- Rent paid on 5th → **Cash outflow**
- EMI paid on 10th → **Cash outflow**

📌 **Key Insight:** 
Even if monthly income is high, 
if cash comes late → it creates a **liquidity problem**. 
