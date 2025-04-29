# lab-report-analysis


# 🧪 Lab Report Parser API

This is a FastAPI-based service to **extract lab test information** from lab report images.  
It performs **OCR** (Optical Character Recognition) to read the text from images, **parses** the results, and **returns structured JSON** including test names, values, reference ranges, and whether the results are **out of range**.

---

## 📸 Example

**Input Image:**  
(Lab report containing tests like Hemoglobin, WBC Count, etc.)

**API Output:**

```json
[
  {
    "test_name": "Hemoglobin",
    "value": 10.2,
    "unit": "g/dL",
    "reference_range": "13.5 - 17.5",
    "is_out_of_range": true
  },
  {
    "test_name": "WBC Count",
    "value": 11500,
    "unit": "/µL",
    "reference_range": "4000 - 11000",
    "is_out_of_range": true
  }
]



Features
* Image Upload & OCR

* Lab Test Data Extraction

* Range Analysis

*  FastAPI RESTful API
*  Interactive Swagger Docs (/docs)

