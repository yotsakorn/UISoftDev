# UISoftDevTeam



//////------------------------------------------------/////// 
-Requirements 
-Functional requirement  
		-User
			- Login  (น่าจะเอาออก)
			- Logout (น่าจะเอาออก)
			- เลือกจองห้องได้	
			- เลือกอุปกรณ์ที่จะใช้ได้ 	(ถ้าห้องนั้นมี)
			- ตรวจสอบสถานะการใช้งานห้องประชุมแบบ Real-time	(ได้โดยที่ไม่ต้องlogin)
			- เพิ่ม ลบ แก้ไข การจอง สือค้นข้อมูลห้องประชุมและข้อมูลการยืมอุปกรณ์ห้องประชุมได้
			- ตรวจสอบรายละเอียดการจองใช้งานห้องประชุมที่เลือกไว้ได้  
			- มีระบบค้นหาห้องที่ตรงตามความต้องการ (ได้โดยที่ไม่ต้องlogin)
			-ใส่จำนวนคน
			-เลือกอุปกรณ์
			-เลือกระยะเวลา 
			-เลือกช่วงเวลา (ใส่ไม่ใสก็ได้) 
			-เลือกวัน
			
		-Admin
			- กำหนดสิทธิ์การใช้งานของผู้ใช้ระบบได้
			- สามารถกำหนดและแก้ไขค่าต่าง ๆ ของระบบได้ 
			- สามารถเพิ่ม ลบ แก้ไข สืบค้นข้อมูลต่างๆ ของระบบได้
			- ยกเลิกการจองห้องของ user / check out
			- ปิดห้องให้ไม่สามารถจองได้ (เช่น มีอุปกรณ์ภายในห้องเสีย ห้องนั้นจะไม่สามารถใช้งานได้จนกว่าจะได้รับการซ่อมเเซม แอดมินจะไปกด)
			- ปรับเปลี่ยนลักษณะของห้องได้(เช่น เพิ่ม-ลดอุปกรณ์, จำนวนที่นั่งในห้อง)
      
-Non-functional requirement (ข้อกำหนดด้านการ ใช้งาน)
		User
		- login ด้วยรหัส new acis
    		- จองห้องล่วงหน้าได้ไม่เกิน 7 วัน
      		- เมื่อมีการเปลี่ยนเเปลงในระบบ ไม่ว่าจะเป็นการจอง, ยกเลิกการจอง หรือมีการปรับเปลี่ยนอุปกรณ์ภายในห้อง จะต้องมีการupdateสถานะของห้องนั้นๆให้เร็วที่สุด
      		- สามารถยกเลิกได้ตลอกเวลา
      		- จองห้องได้วันละไม่เกิน 4 ชม.
      		- ถ้าถึงเวลาที่จองเเล้วเเต่ยังไม่มาcheck inภายใน 15 นาที การจองจะถูกยกเลิก
		Admin
     		- หลังจากยกเลิกการจองของuserต้องมีemailไปแจ้งuser(จะเอาอีเมลจากไหน เดี๋ยวคิดกันอีกที)
