# 🏨 Hotel Booking Data Analysis  
## Understanding Guest Behavior, Cancellations & Revenue Opportunities (EDA)  
**Prepared By: Milin Rao Deshmukh**

---

## 📌 Project Overview  
This project analyzes **hotel booking behavior** using a dataset of over **119,390 booking records**.  
The objective is to uncover insights related to:

- Cancellation patterns  
- Pricing behavior  
- Stay duration & seasonality  
- Guest demographics  
- Booking channels & customer types  
- Revenue opportunities  

Through structured EDA, feature engineering, segmentation, and statistical insights, the project identifies key factors that influence cancellations and reveals opportunities to reduce revenue loss and improve guest experience.

---

## 📊 Dataset Summary  

- **Rows:** 119,390  
- **Columns:** 32  
- **Hotel Types:** City Hotel & Resort Hotel  
- **Duration:** ~2.5 years  

### **Key Features**
- Guest demographics (country, guest type, repeat status)  
- Booking details (lead time, ADR, nights, special requests)  
- Stay information (dates, stay length)  
- Market segments & distribution channels  
- Cancellation flag & deposit type  

### **Tools Used**
- **Python**
  - Pandas  
  - NumPy  
  - Matplotlib  
  - Seaborn  

---

## 🧹 Data Cleaning & Preparation  

### ✔ **Handling Missing Values**
- `children` → filled with **0**  
- `country` → filled with **"Unknown"**  
- `agent`, `company` → filled with **0**, converted to **integers**

### ✔ **Correcting Data Types**
- Converted arrival date fields to **datetime**  

### ✔ **Removing Duplicates**
- Removed **~900 duplicate rows**

### ✔ **Feature Engineering**
Created additional analytical fields:
- `stay_length`  
- `total_guests`  
- `year_month`  
- `length_of_stay`  
- Domestic vs International segmentation  
- Arrival day of week  

---

## 🔍 Exploratory Data Analysis (EDA)  
### **Key Findings**
- City Hotels receive more bookings but also have **higher cancellations**  
- Transient guests cancel most; repeat guests cancel the least  
- **More special requests = lower cancellation risk**  
- OTA (Online Travel Agents) → highest cancellations  
- International guests are more profitable & reliable  
- Longer lead time strongly correlates with cancellation  
- July–August peak months show volatility  
- ADR changes significantly across hotel type, guest type, and channel  

---

## 🧪 In-Depth Statistical & Behavioral Insights  

### 1️⃣ **Hotel Type Performance**

| Hotel Type   | Cancellation Rate | ADR    |
|--------------|-------------------|--------|
| City Hotel   | Higher            | Higher |
| Resort Hotel | Lower             | Lower  |

**Insight:** City Hotels earn more but face higher cancellation risk.

---

### 2️⃣ **Deposit Type Impact**
- **No Deposit:** 26.7% cancellation  
- **Refundable:** 24.3%  
- **Non-Refund:** 94.7% (suspiciously high)  

**Insight:** Non-refundable category requires further validation.

---

### 3️⃣ **Lead Time Influence**
- Canceled bookings → **~106 days** lead time  
- Non-canceled → **~70 days**  

**Insight:** Longer lead time increases cancellation likelihood.

---

### 4️⃣ **Guest Type Impact**
- **Transient guests:** Highest cancellations  
- **Repeat guests:** Lowest cancellations (~7.6%)  

**Insight:** Loyalty is a strong predictor of reliability.

---

### 5️⃣ **Special Requests**
- **0 requests:** 33% cancellation  
- **3+ requests:** Less than 17%  

**Insight:** More special requests = stronger booking intent.

---

### 6️⃣ **Market Segment Impact**
- Highest cancellations → **OTA**  
- Lowest cancellations → **Corporate & Complementary**

**Insight:** OTA bookings require stricter confirmation rules.

---

### 7️⃣ **International vs Domestic**
**International guests:**
- Cancel less  
- Book earlier  
- Stay longer  
- Spend more  
- Make more requests  

**Insight:** International guests are high-value and reliable.

---

### 8️⃣ **Day of Week Impact**
- Highest cancellations → **Friday & Saturday**  
- Lowest → **Tuesday**  

**Insight:** Weekend bookings are more volatile.

---

## 🗂️ Objective Question Outcomes (Short Summary)
- Average lead time:  
  - Canceled → **105 days**  
  - Non-canceled → **70 days**  
- Most booked month → **August**  
- Highest ADR → Transient guests  
- Avg. special requests → **0.69 per booking**  
- Highest ADR channel → **GDS**  
- Lead time vs stay length correlation → **0.31**  
- Bookings with children/babies → **9,103**  
- Repeat guests lead time → **17 days**  
- Most common room mapping → **('A', 'A')**

---

## 💡 Key Insights Summary  
- Long lead time = high cancellation risk  
- Repeat guests and special requests indicate strong commitment  
- OTA bookings are the riskiest  
- International guests deliver consistent revenue  
- Summer months have high bookings & cancellations  
- City Hotels must address high cancellation patterns  
- Non-refundable category may reflect data or operational issues  

---

## 🚀 Recommendations  

### 🔷 Reduce Cancellations  
- Target long lead-time bookings with reminders  
- Review City Hotel policies to reduce cancellations  
- Investigate high cancellation rates in “Non-Refund” type  

### 🔷 Strengthen Loyalty  
- Reward repeat guests  
- Offer benefits to convert first-time guests  

### 🔷 Optimize Market Segments  
- Add stricter confirmation for OTA bookings  
- Promote corporate & group stays  

### 🔷 Improve Guest Experience  
- Prepare early for special requests  
- Provide multilingual support  
- Focus on international guest preferences  

### 🔷 Smart Revenue Strategies  
- Apply dynamic pricing for summer months  
- Use early-bird and last-minute offers  
- Slightly overbook during high-cancellation seasons  

---

## 🏁 Conclusion  
This project converts raw hotel booking data into actionable insights that help:

- Reduce cancellations  
- Improve revenue consistency  
- Understand guest behavior  
- Build targeted customer strategies  
- Enhance operations  

Through detailed EDA and behavioral analysis, hotels can anticipate cancellations, optimize pricing, and deliver better guest experiences—turning data into effective business decisions.

---

## 🛠️ Tech Stack  
- **Python**  
- **Pandas**  
- **NumPy**  
- **Matplotlib / Seaborn**  
- **EDA & Feature Engineering**  
- **Data Visualization**
