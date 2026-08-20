**Automated Gear Defect Inspection & Sorting System**
An end-to-end industrial automation and edge AI prototype designed to detect and physically sort defective 3D-printed gears on an active conveyor line. The system pairs a fine-tuned YOLOv8-nano model on a Raspberry Pi 5 with a custom rack-and-pinion rejection mechanism to deliver real-time visual inspection without human intervention. 
**Key Features & Highlights**
Edge AI Vision Pipeline: Processes live 1080p video streams via OpenCV on a Raspberry Pi 5, running a lightweight YOLOv8-nano network to classify gears into defective and non-defective states. 
Automated Physical Sorting: When defect confidence exceeds 0.75, GPIO-triggered PWM signals drive an MG995 servo to power an 80 mm linear rack-and-pinion stroke, lateral-ejecting faulty gears in under 150 ms.  
High-Throughput Performance: Achieves 94.6% mAP@0.5 and an overall 92% physical sorting accuracy with a 312 ms end-to-end cycle latency (~12 gears/min). 
Cost-Efficient Embedded Architecture: Built for under ₹17,000 using accessible embedded hardware, 3D-printed components, and low-power operations (~14.3 W).  
**Tech Stack & Hardware**
**AI & Computer Vision:** Python, YOLOv8 (Ultralytics), OpenCV, Roboflow  
**Compute & Hardware:** Raspberry Pi 5 (4GB RAM, Quad-core Cortex-A76), USB Camera (1080p, 30fps)  
**Actuation & Mechanics:** MG995 Servo Motor, 12V DC Geared Motor, 3D-printed Conveyor Belt & Rack-and-Pinion Ejector 
