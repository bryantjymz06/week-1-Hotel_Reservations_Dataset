## **Hotel Booking Cancellation Analysis**

### **1. Project Overview**

This project explores a hotel booking dataset to understand the factors that influence booking cancellations. The goal at this stage is to perform exploratory data analysis (EDA), identify important patterns, and prepare the dataset for future modelling.

---

### **2. Setup and Environment**

This project is using:

- Python 3.x
- Jupyter Notebook
- pandas, numpy
- seaborn, matplotlib

To install dependencies:
pip install pandas numpy seaborn matplotlib scikit-learn

### **3. Dataset Understanding**

The dataset contains **36,275 booking records**, each representing a single hotel reservation.
Key feature groups include:

- **Guest details:** adults, children, repeated guest
- **Stay details:** weekend nights, week nights, room type
- **Booking behaviour:** lead time, previous cancellations, previous non‑cancellations
- **Timing:** arrival year, month, date
- **Target variable:** `booking_status` (0 = Not Cancelled, 1 = Cancelled)

A missing‑value check (`df.isna().sum()`) confirmed that the dataset contains **no missing values**.

---

### **4. Initial Observations (EDA Summary)**

Early analysis revealed several important patterns:

- **Lead time** is significantly higher for cancelled bookings (≈139 days vs 59 days).
- **Repeated guests** almost never cancel, suggesting strong loyalty behaviour.
- **Cancelled bookings** tend to involve slightly longer stays (more nights).
- **Car parking requests** are more common in non‑cancelled bookings, indicating stronger commitment.
- **Arrival year** contains only 2017, so it has no predictive value.
- Correlation analysis shows meaningful relationships between lead time, previous cancellations, and booking status.

These insights will guide feature selection and modelling in the next stage.

---
