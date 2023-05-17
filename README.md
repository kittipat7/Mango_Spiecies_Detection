# Mango_Spiecies_Detection
## วัตถุประสงค์
สร้าง object detection model สำหรับ การแยกสายพันธ์ุมะม่วง
## Data
ข้อมูลมะม่วงจากตลาดไททั้งหมดสามสายพันธุ์ ได้แก่ 1. เขียวเสวย 167 ลูก, 2. แก้วขมิ้น 186 ลูก, 3.น้ำดอกไม้ 15 ลูก รวม 368 ลูก
## วิธีที่ใช้
- ทำการตีกรอบรูปภาพโดยและแบ่ง train 70,val 15, test 15 โดย https://roboflow.com/
- ใช้ Model Objct Detection YOLO ในการสร้าง model และวัดผลโดย Mean Average Precision (mAP)
- mAP สามารถวัดผลได้ทั้ง accuracy ของการตีกรอบ object detection และการ label class
- เปรียบเทียบ model YOLOv5, YOLOv8 50 epoch และ 75 epoch

## ตัวอย่างผลลัพธ์การนำไปใช้งาน
![75](https://github.com/kittipat7/Mango_Spiecies_Detection/assets/97491541/789baa86-3726-433f-a7cd-0ea1b2e5ebb8)

## สรุปผล
### validation set

![image](https://github.com/kittipat7/Mango_Spiecies_Detection/assets/97491541/0ad2a6ce-942b-433e-b287-86d97e6b6ca2)  ![image](https://github.com/kittipat7/Mango_Spiecies_Detection/assets/97491541/0d70e468-557d-4d83-838e-0b77d5f3542e)


จากผลลัพธ์ที่ได้พบว่าตัว YOLOv8 มีประสิทธิภาพที่สูงกว่า YOLOv5 โดย YOLOv8 มี mAP50 อยู่ที่ 0.995 และมี mAP50-95 อยู่ที่ 0.954

## Reference
https://roboflow.com/

https://github.com/ultralytics/yolov5

https://github.com/ultralytics/ultralytics
