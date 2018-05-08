# ฐานข้อมูลจังหวัด

เป็นไฟล์ .sql นะครับ ซึ่งภายในประกอบไปด้วย

  - ภาค
  - ชื่อจังหวัด
  - อำเภอ
  - ตำบล
  - รหัสไปรษณีย์
  - รหัสจังหวัด, อำเภอ
  - ชื่อ จังหวัด, อำเภอภาษาอังกฤษ


## ตารางข้อมูล



**geographies**

|Field |Type |Key|
|----------------|-------------------------------|-----------------------------|
|id|Integer|PK|
|name|Varchar(255)||

----------


**provinces**

|Field |Type |Key|
|----------------|-------------------------------|-----------------------------|
|id|Integer|PK|
|code|Varchar(150)||
|name_th|Varchar(150)||
|name_en|Varchar(150)||
|geography_id|Integer||


----------


**amphures**

|Field |Type |Key|
|----------------|-------------------------------|-----------------------------|
|id|Integer|PK|
|code|Varchar(4)||
|name_th|Varchar(150)||
|name_en|Varchar(150)||
|province_id|Integer||

----------

**districts**

|Field |Type |Key|
|----------------|-------------------------------|-----------------------------|
|id|Integer|PK|
|zip_code|Integer||
|name_th|Varchar(150)||
|name_en|Varchar(150)||
|amphure_id|Integer||



## อ้างอิงจาก

- [www.ssckp.org](http://www.ssckp.org/information-technology-for-crewphra-news/79-temples-tumbons-districts-amphures-77-provinces-database)
- อื่นๆ (หลายที่เหลือเกิน)



