# Mango_Spiecies_Detection
## วัตถุประสงค์
สร้าง object detection model สำหรับ การแยกสายพันธ์ุมะม่วง
## Data
ข้อมูลมะม่วงจากตลาดไททั้งหมดสามสายพันธุ์ ได้แก่ 1. เขียวเสวย 167 ลูก, 2. แก้วขมิ้น 186 ลูก, 3.น้ำดอกไม้ 15 ลูก รวม 368 ลูก
## วิธีที่ใช้
- ทำการตีกรอบรูปภาพโดยและแบ่ง train 70,val 15, test 15 โดย https://roboflow.com/
- ใช้ Model Objct Detection YOLO ในการสร้าง model และวัดผลโดย Mean Average Precision (mAP)
- เปรียบเทียบ model YOLOv5, YOLOv8 50 epoch และ 75 epoch
![75](https://github.com/kittipat7/Mango_Spiecies_Detection/assets/97491541/789baa86-3726-433f-a7cd-0ea1b2e5ebb8)
	mAPE 50-95	
	50	75
YOLOv5	0.909	0.943
YOLOv8	0.804	0.878
