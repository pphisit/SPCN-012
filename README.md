# SPCN-012
 # Hypervisor Technology
 ### hypervisor คือ 
 เทคนิคการจำลองให้ระบบปฎิบัติการหลายระบบทำงานพร้อมกันได้ โดยหน้าที่การทำงานก็คิอ การตั้งค่าให้แต่ละระบบปฎิบัติการไม่ให้ทำงานทับช้อนกัน โดย hypervisor มีอีกชื่อเรียกก็คือ 
 Virtual Machine Management (VMM)
 
 โดยคลัสเตอร์การคำนวณ, การคำนวณแบบกริด, พีซีหรือเมนเฟรมซึ่งมีอยู่ในคอมพิวเตอร์ทุกประเภทแต่จะมีระบบที่แตกต่างกัน เนื่องจากแต่ละระบบ ได้ถูกออกแบบตามความต้องการของระบบนั้นๆ แต่ hypervisor เหมาะกับเมนเฟรมมากว่า windows OS เพราะว่า hypervisor ต้องจัดการระบบพร้อมกับเหมือบกับโฮสต์
ประโยชน์สำคัญของ Hypervisor 
ประโยชน์ที่สำคัญของ Hypervisor คือความปลอดภัย ถ้าอยากทดสอบอะไรที่มีความเสี่ยง หรือเป็นอันตรายต่อคอมพิวเตอร์ สามารถทดสอบบน Hypervisor ได้เพราะว่าทุกอย่างบน Hypervisor ไม่ส่งผลต่อคอมพิวเตอร์ที่ใช้อยู่

อ้างอิง https://personet.co.th/hypervisor/
# Container Technology
เป็นกระบวนการปรับใช้ซอฟต์แวร์ที่รวมแอปพลิเคชันเข้ากับไฟล์และไลบรารีทั้งหมดที่จำเป็นสำหรับการทำงาน

ประโยชน์ของการคอนเทนเนอร์คืออะไร
* ความสามารถในการเคลื่อนย้าย
ใช้ในสภาพแวดล้อมได้หลากหลาย โดยไม่ต้องเขียนโปรแกรมใหม่ สร้างเพียงครั้งเดียวแต่สามารถปรับใช้บนหลายระบบปฎิบัติการ 
* ความคล่องตัว
สามารถแก้ไขหรือปรับแต่งอะไรก็ได้ โดยที่จะไม่รบกวนต่อระบบอื่นๆที่ใช้อยู่ 
* ความทนทานต่อความเสียหาย
สร้างคอนเทนเนอร์หลายๆตัวเพื่อป้องกันความเสียหาย เพราะคอนเทนเนอร์ทำงานแบบแยกกัน ถ้ามีคอนเทนเนอร์ที่ผิดพลาด จะไม่ส่งผลกระทบต่อคอนเทนเนอร์อื่นๆ

ตัวอย่างการใช้งาน Container
* นำเทคโนโลยียุคก่อน เช่น Java, .NET หรือ PHP เพื่อรันบนพื้นฐานยุคใหม่
* แก้ปัญหาเรื่อง system dependency ระหว่างแอพแต่ละเวอร์ชัน

อ้างอิง https://www.blognone.com/node/105928
https://aws.amazon.com/th/what-is/containerization/
# Monolithic MicroService
Monolithic คือ สถาปัตยกรรมที่นิยมโดยทั่วไปถูกเขียนขึ้นมาด้วย Environment เดียวกันใช้ Database เดียวกัน จะพบเห็นใน Web Application ทั่วไป การพัฒนาอาจจะแบ่งการทำงานโดยมี ทีมหน้าบ้าน ทีมหลังบ้าน และทีม Database 

ประโยชน์ของ Monolithic
* ง่ายต่อการ Scale การ Scale สามารถทำได้โดย Clone Application นี้ออกมาเป็น Server ที่ 2 หรือ 3 และใช้ Load balancer ทำหน้าที่ Balance ให้อีกครั้งหนึ่ง

Microservices คือ สถาปัตยกรรมหรือเทคนิคการพัฒนาซอฟต์แวร์ 
แยก Component ออกมาเป็น Collection แบ่งตาม Business Capability หรือตาม Sub Domain ขึ้นอยู่กับจุดประสงค์ของงานในส่วน Database ก็เช่นกัน

ประโยชน์ของ Microservices เช่น
* แก้ไขปัญหาความซับซ้อนของ Application

อ้างอิง https://www.softnix.co.th/2018/07/13/%E0%B8%82%E0%B9%89%E0%B8%AD%E0%B9%81%E0%B8%95%E0%B8%81%E0%B8%95%E0%B9%88%E0%B8%B2%E0%B8%87%E0%B8%A3%E0%B8%B0%E0%B8%AB%E0%B8%A7%E0%B9%88%E0%B8%B2%E0%B8%87-microservices-%E0%B9%81%E0%B8%A5%E0%B8%B0-mono/
# Proxmox
Proxmox คือ เป็นแพลตฟอร์มจัดการเซิร์ฟเวอร์แบบโอเพ่นซอร์ซ สำหรับการจำลองเสมือนขององค์กร  พัฒนาในออสเตรียภายใต้ Internet Foundation of Austria 
สามารถปรับใช้และจัดการ vm และคอนเทนเนอร์ได้
จุดเด่นของ Proxmox

จุดเด่นของ Proxmox

* สามารถบริหารจัดการหรือสร้าง Environment ได้อย่างรวดเร็ว
* มีประสิทธิภาพสูง
* ประหยัดงบประมาณ ช่วยลดค่าใช้จ่ายที่ไม่จำเป็นออกไป

Proxmox เหมาะกับใคร

* เหมาะกับองค์ที่ต้องการใช้ระบบ Server Virtualization ที่ใช้ Private Cloud 

อ้างอิง https://www.quickserv.co.th/knowledge-base/technology/VMware-vSphere-%e0%b8%81%e0%b8%b1%e0%b8%9a-Proxmox-%e0%b8%aa%e0%b8%b3%e0%b8%ab%e0%b8%a3%e0%b8%b1%e0%b8%9a%e0%b8%98%e0%b8%b8%e0%b8%a3%e0%b8%81%e0%b8%b4%e0%b8%88-%e0%b9%83%e0%b8%8a%e0%b9%89%e0%b9%81%e0%b8%9a%e0%b8%9a%e0%b9%84%e0%b8%ab%e0%b8%99%e0%b8%94%e0%b8%b5%e0%b8%97%e0%b8%b5%e0%b9%88%e0%b8%aa%e0%b8%b8%e0%b8%94/
# Ceph

 คือ Software ที่เอาไว้ใช้งานในการทำ Storage Pool โดยDisk ที่เอามาใช้งาน ไม่จำเป็นที่จะต้องมีขนาดเท่ากันทุกลูก และไม่ต้องเป็น Disk ประเภทเดียวกัน ทำให้Ceph มีความยืดหยุ่นมากกว่า RAID 

 Ceph จะประกอบด้วยส่วนประกอบหลัก ๆ 3 ส่วน คือ
* MON (Monitor Node) ทำหน้าที่ดูแลสถานะของ Ceph cluster
* OSD (Object Storage Node) เป็น Node ทำหน้าที่เก็บข้อมูล ของระบบ
* MDS (Metadata Node) ทำหน้าที่ดูแลสถานะของ file hierarchy 


ข้อดี
* เป็น Open source ไม่มีค่าใช้จ่ายสำหรับตัวซอฟต์แวร์
* สามารถขยายระบบได้ง่าย เพียงเติมเครื่องเข้าระบบ
* ใช้ Hardware ทั่ว ๆ ไป ไม่จำเป็นต้องเป็น Hardware เฉพาะ

ข้อเสีย
* จะเปลืองดิสก์กว่า Storage แบบปกติ

อ้างอิง https://www.clusterkit.co.th/blogs/ceph-storage/
# NFS
NFS ย่อมาจาก Network File System 

เป็นตัวช่วยให้สามารถแชร์ข้อมูลผ่านLocal Networkได้ ถูกใช้งานเมื่อ ค.ศ.1984 แต่ยังมีการใช้กันอย่างแพร์หลายถึงปัจจุบัน
NFS ใช้รูปแบบโครงสร้างที่เป็น Server และ Client ในการทำให้คอมพิวเตอร์หลาย ๆ เครื่องใน Local Network เดียวกันสามารถเข้าถึงไฟล์ได้
โดยฝั่งของ Server จะทำการตั้งค่า Folder ว่า Folder ไหนจะทำการแชร์ผ่าน Network ฝั่งของ Client ก็จะต้อง Mount ไฟล์ผ่าน Network โดยใช้คำสั่ง Mount

ในอดีต NFS เป็นที่นิยมใช้งานกันบน Unix และ Linux
เนื่องจาก NFS ถูกพัฒนาโดย Sun Microsystems ซึ่งเป็นบริษัทที่เป็น Vendor ของ Unix 
ปัจจุบัน NFS Protocol ได้กลายเป็น Standard Protocol ที่ง่ายต่อการใช้งานและในปัจจุบันสามารถที่จะใช้งานกับ Windows ได้

อ้างอิง https://blog.cloudhm.co.th/nfs-vs-smb/
