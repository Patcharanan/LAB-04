#นายพชรนันท์ จันทร์รักษ์ 57030198
#ใบงานที่ 4
เรื่อง การใช้งานคำสั่งเกี่ยวกับการแสดงผลบน Text Mode ขั้นพื้นฐานในภาษา C#
##วัตถุประสงค์
1. เพื่อให้นักศึกษาบอกชื่อ method ที่ใช้ในการแสดงผลบน Text Mode ขั้นพื้นฐานในภาษา C# ได้
2. เพื่อให้นักศึกษาสามารถใช้คำสั่งแสดงผลทางหน้าจอ เบื้องต้นได้

##ลำดับขั้นการทดลอง
###การเตรียมการก่อนการทดลอง
  * เปิดโปรแกรม Visual Studio 
  *  เลือก File >>New Project >> เลือก Console Application 
![P1](https://github.com/Desktop-Programming-Lab-2559/LAB-04/blob/master/imgs/P1.png)
  *  ช่อง Name ใส่ชื่อของ project (ในที่นี้คือ Lab4)
  *  ช่อง Location ใส่ชื่อ folder ที่เป็นที่ตั้งของ Project (ในที่นี้ สมมติเป็น E:\vslab)
  *  ช่อง Solution name ให้ใส่ชื่อ Solution โดยปกติก็ให้ปล่อยไว้อย่างนั้น 
  *  กดปุ่ม OK โปรแกรม Visual Studio จะสร้าง project ชื่อ “lab4”ภายใต้ solution “lab4” และไฟล์ lsb4.cs ซึ่งมี source code ดังรูป 

![P2](https://github.com/Desktop-Programming-Lab-2559/LAB-04/blob/master/imgs/P2.png)

ส่วนสำคัญของโปรแกรม lab4.cs  คือบรรทัดที่ 1 “using System” และเมธอด Main(string[] args)


 *  ให้ลบ source code ในบรรทัดที่ 2-5 ออกไปก่อน เนื่องจากเป็น assembly ที่ไม่จำเป็นต่อการทำงานของโปรแกรม 

## 1. การทดลองเมดธอด Console.Write()
* ให้เพิ่ม บรรทัดต่อไปนี้ลงไปในในเมธอด Main()
```csharp 
    Console.Write(“Hello”);
```
ดังปรากฏในบรรทัดที่ 9 ของรูปด้านล่าง 

![](https://github.com/Desktop-Programming-Lab-2559/LAB-04/blob/master/imgs/P3.png)
 
 * สั่ง Run โปรแกรม เพื่อดูผลการทดลอง 

####บันทึกผลการทดลอง
![](https://raw.githubusercontent.com/Patcharanan/LAB-04/07f5e27fc1cad6a8962050c7b68d16b2d1034e88/imgs/1.PNG)

* จากผลการทดลองพบว่า ตอนรันผลจะแสดงคำว่า Hello ออกมา
<hr> 


แก้ไขโปรแกรม ให้เป็นดังรูปด้านล่างนี้    

![](https://github.com/Desktop-Programming-Lab-2559/LAB-04/blob/master/imgs/P4.png)

 * สั่ง Run โปรแกรมและบันทึกผลที่ได้จากการรันโปรแกรม
 * การรันแล้วทำให้หน้าจอ console ยังคงแสดงผลค้างอยู่นั้น ให้เลือกเมนู Debug -> Start Without Debugging (Ctrl+F5) มิฉะนั้น หน้าจอ console จะหายไปอย่างรวดเร็ว
 ![](https://raw.githubusercontent.com/Patcharanan/LAB-04/ea023dbbbc45a017fdd0b2f776ab446d9360ef8d/imgs/2.PNG)
 
* จากผลการทดลองพบว่า เมื่อกดรันโปรแกรมจะแสดงคำว่า Hello World ออกมา
<hr>


### คำถาม 4.1 

ผลที่ได้จากการทดลอง เป็นอย่างที่นักศึกษาคิดหรือไม่ อย่างไร  จงอธิบาย
* เป็นอย่างที่คิด คือเมื่อใช้ฟังก์ชันให้เขียนคำว่าอะไรออกมา โปรแกรมก็จะแสดงคำที่พิมลงไปออกมาแสดงผล 
<hr>


## 2. การทดลองเมดธอด Console.WriteLine()

แก้โปรแกรมในเมดธอด Main() ให้เป็นดังรูปต่อไปนี้

![](https://github.com/Desktop-Programming-Lab-2559/LAB-04/blob/master/imgs/P5.png)

 * สั่ง Run โปรแกรม เพื่อดูผลการทดลอง 

บันทึกผลที่ได้จากการรันโปรแกรม
![](https://github.com/Patcharanan/LAB-04/blob/master/imgs/3.PNG?raw=true)

แก้ไขโปรแกรม ให้เป็นดังรูปด้านล่างนี้

![](https://github.com/Desktop-Programming-Lab-2559/LAB-04/blob/master/imgs/P6.png)

 * สั่ง Run โปรแกรมและบันทึกผลที่ได้จากการรันโปรแกรม

![](https://github.com/Patcharanan/LAB-04/blob/master/imgs/4.PNG?raw=true)

###คำถาม 4.2

ผลที่ได้จากการทดลอง เป็นอย่างที่นักศึกษาคิดหรือไม่ อย่างไร  จงอธิบาย

 * เป็นอย่างคิดคือ ฟังก์ชัน WriteLine เมื่อจบประโยคจะทำการเว้นบรรทัดลงมา ผลเป็นไปตามการทดลอง

### คำถาม 4.3 

จงอธิบายความแตกต่างระหว่างคำสั่ง Console.Write() และ Console.WriteLine()

 * Console.Write() เมื่อทำการรันโปรแกรม ประโยคจะติดๆกันไปเรื่อยๆ ไม่มีการเว้นรรทัดให้ แต่ Console.WriteLine() เมื่อจบประโยคจะเว้นบรรทัดแล้วขึ้นต้นประโยคให้

##สรุปผลการทดลอง

* จากผลการทดลองพบว่า ฟังก์ชัน Console.Write() และ Console.WriteLine() ต่างกันตรงที่ Console.Write() จะไม่มีการเว้นบรรทัดเมื่อจบประโยค แต่ Console.WriteLine() จะทำการเว้นบรรทัด 

#นายพชรนันท์ จันทร์รักษ์ 57030198
