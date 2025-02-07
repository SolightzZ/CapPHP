# ระบบจัดการข้อมูลสายพันธุ์แมว  

![GitHub all releases](https://img.shields.io/github/downloads/SolightzZ/Device-Info-Add-on/total)
![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/Device-Info-Add-on)

## คำอธิบาย  
โปรเจกต์นี้เป็นระบบจัดการข้อมูลสายพันธุ์แมว โดยมีระบบ Back-end สำหรับผู้ดูแล (Admin) และระบบ Front-end สำหรับผู้ใช้ทั่วไป  

## โครงสร้างฐานข้อมูล  
ตาราง `CatBreeds` ใช้สำหรับเก็บข้อมูลเกี่ยวกับสายพันธุ์แมว  

```sql
CREATE TABLE CatBreeds (  
    id INT AUTO_INCREMENT PRIMARY KEY,   
    name_th VARCHAR(255) NOT NULL,   
    name_en VARCHAR(255) NOT NULL,   
    description TEXT NOT NULL,   
    characteristics TEXT,   
    care_instructions TEXT,   
    image_url VARCHAR(2083),   
    is_visible TINYINT(1) NOT NULL DEFAULT 1  
);
