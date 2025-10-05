# RaspberryPi-SelfDriving-Logistics
DDongkey – Raspberry Pi-based AI autonomous driving car for warehouse inventory management and logistics automation.

**Project Duration:** April 1, 2021 – April 20, 2021  

---

## Project Overview  
**Dongkey** is an **autonomous inventory management robot** that leverages AI and self-driving technology for efficient warehouse operations.  
It navigates warehouses, automatically detects inventory, calculates required stock, and generates management reports.  

- **Lane Detection**: Autonomous navigation inside warehouses  
- **Object Detection (YOLOv4)**: Inventory recognition & quantification  
- **RPA (Robotic Process Automation)**: Automated reporting and documentation  

### Motivation  
- Over **30% of domestic logistics centers are outdated** → Smart warehouse transition needed  
- Post-COVID-19 logistics boom → Higher demand for efficient inventory management  
- Growing **global logistics robot market** → Domestic adoption becoming essential  

### Objectives  
- Improve **accuracy & efficiency** of inventory inspection  
- Reduce **time and cost** of warehouse operations  
- Enable **real-time and continuous monitoring**  

---

## System Architecture  

1. **Autonomous Navigation**  
   - Raspberry Pi-based robot  
   - Lane Detection for rail tracking  
   - Stops at warehouse entry upon **red line detection**  

2. **Inventory Recognition**  
   - Captures images via Webcam → Transfers via SCP  
   - YOLOv4 Object Detection → Identifies items & calculates shortages  
   - Updates warehouse DB  

3. **Automated Reporting**  
   - Generates reports with stock status & required actions  
   - Uses RPA for document creation & printing  

---

## Related Research  
- **YOLOv4**: Balancing speed and accuracy for real-time detection  
- **OpenCV-based Lane Detection**: Using Canny Edge & Hough Transform  
- **Autonomous Driving Hardware**: PCA9685, DC motors, PWM-based control  

---

## Technologies  

- **Hardware Control**: Raspberry Pi, GPIO, Servo/DC Motor  
- **Computer Vision**: OpenCV, Lane Detection  
- **Object Detection**: YOLOv4 (1,500+ labeled images → 10,000 augmented)  
- **Server Communication**: Socket & SCP (SSH)  
- **DB & RPA**: Automated report generation  

---

## Limitations  
- Current navigation requires **red line detection** to stop (low practicality)  
- Data integration failed after multi-threaded sensor streaming  

---

## Future Improvements  
- Replace red line detection with **direct warehouse recognition**  
- Optimize computation with **additional Raspberry Pi** or unified processing  
