---

## Difference Between Total, Direct, and Derived Currency Amounts

In SAP Analytics Cloud (SAC) and finance reporting, currency values are often categorized as **Direct**, **Derived**, and **Total** amounts to clearly track how values are calculated.

---

## 1️⃣ Direct USD / EUR / AUD

### Meaning
- **Direct** amounts are values that are **entered or loaded directly** in that currency.
- No currency conversion is applied.

### Characteristics
- Original transaction currency
- Comes from source system (BW / S/4HANA) or manual input
- Most reliable raw data

### Example
- Invoice created in **USD**
  - Direct USD = 10,000
  - Direct EUR = 0
  - Direct AUD = 0

---

## 2️⃣ Derived USD / EUR / AUD

### Meaning
- **Derived** amounts are calculated by **converting Direct amounts** from another currency.
- Uses **exchange rates** (TCURR / SAC rate models).

### Characteristics
- System-calculated
- Depends on exchange rate and conversion logic
- Used for reporting consistency

### Example
- Invoice entered in **EUR = 9,000**
- Exchange rate: 1 EUR = 1.1 USD

Direct EUR   = 9,000 Derived USD  = 9,900 Derived AUD  = calculated using AUD rate

---

## 3️⃣ Total USD / EUR / AUD

### Meaning
- **Total** amount is the **sum of Direct + Derived amounts** for that currency.

### Characteristics
- Final reporting figure
- Represents complete value in one currency
- Used in dashboards and cash flow reports

### Formula

Total Currency = Direct Currency + Derived Currency

### Example (USD)

Direct USD  = 10,000 Derived USD = 9,900

Total USD   = 19,900
