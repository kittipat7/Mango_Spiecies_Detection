# Mango_Spiecies_Detection
## วัตถุประสงค์
สร้าง object detection model สำหรับ การแยกสายพันธ์ุมะม่วง
## Data
ข้อมูลมะม่วงจากตลาดไททั้งหมดสามสายพันธุ์ ได้แก่ 1. เขียวเสวย 167 ลูก, 2. แก้วขมิ้น 186 ลูก, 3.น้ำดอกไม้ 15 ลูก รวม 368 ลูก
## วิธีที่ใช้
- ทำการตีกรอบรูปภาพโดยและแบ่ง train 70,val 15, test 15 โดย https://roboflow.com/
- ใช้ Model Objct Detection YOLO ในการสร้าง model และวัดผลโดย Mean Average Precision (mAP)
- เปรียบเทียบ model YOLOv5, YOLOv8 50 epoch และ 75 epoch

## ตัวอย่างผลลัพธ์การนำไปใช้งาน
![75](https://github.com/kittipat7/Mango_Spiecies_Detection/assets/97491541/789baa86-3726-433f-a7cd-0ea1b2e5ebb8)

## สรุปผล
![image](https://github.com/kittipat7/Mango_Spiecies_Detection/assets/97491541/e3ed6b80-42e9-4402-8a82-f50b2306c7a1) 	![image](https://github.com/kittipat7/Mango_Spiecies_Detection/assets/97491541/113916c7-251a-492d-baa1-82a6cef9a661)

