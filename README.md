## Resoloute_AI_TASK3
# 🚶‍♂️ Crowd Detection using YOLOv8 – Task 3

This project is part of **Resolute AI's Internship Assignment – Task 3**, which focuses on detecting **crowd presence in videos** using real-time object detection techniques.

The objective is to identify **scenes where three or more people appear** in a frame for **10 or more consecutive frames**, and to output:

- A **CSV file** containing start & end frames of each crowd event
- Saved **image frames with bounding boxes** for visual verification

---

## 🎯 Objective

> Detect the presence of a crowd in video footage using object detection, and log the duration of crowd events to a CSV file. A crowd is defined as:
- **At least 3 people**
- Present for **10 or more consecutive frames**

---

## 🧠 What the App Does

1. Uses the **YOLOv8n model** to detect objects frame-by-frame.
2. Filters only the **'person' class** (class ID `0`).
3. Saves frames where **3+ people** are present.
4. Groups consecutive frames into **crowd events**.
5. Outputs a `crowd_results.csv` file and saves images with bounding boxes.

---

## 🛠️ Tech Stack

| Tool           | Purpose                                  |
|----------------|------------------------------------------|
| YOLOv8 (Ultralytics) | Person detection in video frames        |
| OpenCV         | Video frame reading and image saving     |
| Pandas         | Data logging, analysis, and CSV export   |

---

## 📦 Installation

Clone the repo and install the required libraries:

```bash
pip install -r requirements.txt
