# FitForge – Medical Services Hub (QA Testing Case Study)

## 📌 Project Overview
FitForge is a unified digital healthcare web platform designed to connect patients with nearby doctors, real-time medicine availability, and live consultations.

---

## 🛠️ Tech Stack & Tools Tested
- **Backend & Database:** Python (Flask), SQLite
- **Real-Time Features:** Socket.IO
- **Testing & QA Tools:** Jira, Postman, Google Sheets (Test Cases)

---

## 🧪 QA Responsibilities & Scope
- **Test Case Design:** Created comprehensive manual test cases covering search filters, stock updates, and user registration.
- **Real-Time Chat Testing:** Validated WebSocket connections (Socket.IO) for live patient-doctor consultations to ensure message integrity and low latency.
- **UI/UX & Responsive Testing:** Verified template behavior across Desktop and Mobile viewports.

---

## 📋 Sample Test Case Matrix

| Test Case ID | Feature | Test Scenario | Expected Result | Status |
|-------------|---------|---------------|-----------------|--------|
| TC_FF_001 | Medicine Search | Search for medicine by exact name | System displays list of nearby pharmacies with stock status and prices | PASS |
| TC_FF_002 | Live Consultation | Initiate live chat with doctor | WebSocket connection opens and live message is delivered instantly | PASS |
| TC_FF_003 | Doctor Filter | Filter doctors by location and specialty | Only doctors matching both criteria are displayed | PASS |

---

## 🐛 Sample Bug Report (Jira Format)

- **Bug Summary:** Medicine stock status shows "In Stock" when quantity is 0.
- **Severity:** High | **Priority:** High
- **Steps to Reproduce:**
  1. Navigate to Medicine Search.
  2. Search for item with 0 inventory.
  3. Observe availability tag.
- **Expected Result:** Status should display "Out of Stock".
- **Actual Result:** Status displays "In Stock".
