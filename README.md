# Smart Power Zone Monitor

An AI-powered safety monitoring system for energy facilities, built with YOLOv8, OpenCV, and Streamlit.  
The system detects whether personnel are wearing helmets and safety vests, identifies unauthorized entries,  
and provides real-time alerts to improve safety compliance in high-voltage or restricted zones.

---

## Project Overview

This project simulates an intelligent monitoring system in a power plant or transformer area,  
where safety compliance is crucial. Using computer vision, the model identifies:

- `helmet` → helmet detected  
- `vest` → safety vest detected  
- `no-helmet` → missing helmet  
- `no-vest` → missing vest  
- `person` → any person in the restricted zone  

When a violation (no-helmet / no-vest) is detected, the system highlights it with a red bounding box  
and can optionally play a sound alert or send a notification.

---

## Technical Architecture

| Component     | Description                                             |
|---------------|---------------------------------------------------------|
| Model         | YOLOv8 (Ultralytics)                                    |
| Dataset       | PPE Detection Dataset (Mendeley Data – 3,212 images)   |
| Programming   | Python                                                  |
| Libraries     | OpenCV, Ultralytics, Streamlit, Pandas                 |
| Optional      | Jetson Nano / Raspberry Pi for Edge AI deployment      |

---

### Dataset

This project uses the **PPE Detection Dataset** from Mendeley Data: [https://data.mendeley.com/datasets/zkzghjvpn2/3](https://data.mendeley.com/datasets/zkzghjvpn2/3)  
License: **CC BY 4.0**  
Please cite: Mei-Ling Huang, Ying Cheng, Dataset of Personal Protective Equipment (PPE), Mendeley Data, 2025
