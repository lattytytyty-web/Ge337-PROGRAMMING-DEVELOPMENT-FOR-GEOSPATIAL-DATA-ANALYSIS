# Geospatial Service Area Analysis (Lab 1)

## Overview

โปรเจกต์นี้เป็นส่วนหนึ่งของรายวิชา Geospatial Programming โดยมีวัตถุประสงค์เพื่อเรียนรู้กระบวนการวิเคราะห์ข้อมูลเชิงพื้นที่ (Spatial Analysis) ด้วยภาษา Python และไลบรารีด้าน GIS เช่น GeoPandas, Shapely และ Folium

เนื้อหาในงานประกอบด้วยการสร้างพื้นที่ให้บริการ (Service Area) รอบตำแหน่งสถานีขนส่ง การวิเคราะห์ความสัมพันธ์เชิงพื้นที่กับขอบเขตเขตเมือง และการคำนวณพื้นที่ที่เกี่ยวข้อง

---

## Objectives

* เรียนรู้การจัดการข้อมูลเชิงพื้นที่ประเภท Point และ Polygon
* สร้าง Buffer รอบตำแหน่งสถานีขนส่ง
* วิเคราะห์ Spatial Join ระหว่างพื้นที่ให้บริการและขอบเขตเมือง
* คำนวณพื้นที่ (Area Calculation)
* แสดงผลลัพธ์ในรูปแบบแผนที่เชิงโต้ตอบ

---

## Data Sources

ข้อมูลที่ใช้ในงานเป็นข้อมูลตัวอย่างเพื่อการศึกษาเชิงกระบวนการวิเคราะห์ โดยมีแหล่งที่มาดังนี้

*ข้อมูลตำแหน่งสถานีขนส่ง (Point Data) ได้จากฐานข้อมูล OpenStreetMap (OSM)

*ข้อมูลขอบเขตเขตการปกครอง (Polygon Data) ได้จากฐานข้อมูล OpenStreetMap (OSM) หรือแหล่งข้อมูลสาธารณะ (Open Data) ที่เปิดเผยให้ใช้งานทั่วไป

หมายเหตุ: ข้อมูลถูกนำมาใช้เพื่อวัตถุประสงค์ทางการศึกษาเท่านั้น


---

## Methodology

ขั้นตอนการวิเคราะห์ประกอบด้วย

1. นำเข้าข้อมูลเชิงพื้นที่ด้วย GeoPandas
2. แปลงระบบพิกัด (Coordinate Reference System) ให้เหมาะสม
3. สร้าง Buffer ระยะ 5 กิโลเมตรรอบสถานีขนส่ง
4. วิเคราะห์ Spatial Join ระหว่าง Buffer และขอบเขตเมือง
5. คำนวณพื้นที่ที่อยู่ภายในขอบเขตที่สนใจ
6. แสดงผลลัพธ์ด้วย Matplotlib และ Folium

---

## Results

ผลลัพธ์ของการวิเคราะห์สามารถแสดงในรูปแบบแผนที่ ซึ่งประกอบด้วย

* ตำแหน่งสถานีขนส่ง
* ขอบเขตพื้นที่เมือง
* พื้นที่ Buffer (Service Area)
* ความสัมพันธ์เชิงพื้นที่ระหว่างข้อมูล

---

## Requirements

ไลบรารีที่ใช้ในโปรเจกต์

* geopandas
* shapely
* matplotlib
* folium
* pandas

สามารถติดตั้งด้วยคำสั่ง:

```bash
pip install geopandas shapely matplotlib folium pandas
```

---

## How to Run

1. เปิดไฟล์ Jupyter Notebook (.ipynb)
2. รันโค้ดตามลำดับเซลล์
3. ตรวจสอบผลลัพธ์แผนที่ที่แสดงใน Notebook

---

## Author

Rattiya Phoubon
Student ID: 6606614813

---

## Reference

เอกสารประกอบการเรียน Lab 1: Geospatial Programming and Spatial Analysis
