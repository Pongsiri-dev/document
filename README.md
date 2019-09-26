# รวมคำสั่ง NPM Basic (ช่วยชีวิต)
# เริ่มต้นใช้งาน Node js โดยจะเป็นการสร้างไฟล์ package.json
npm init

# ติดตั้ง modules ที่เราต้องการ
npm install module_name

# อัพเดท modules ที่เราต้องการ ให้เป็นเวอร์ชั่นล่าสุด
npm update module_name

# ถอนติดตั้ง modules ที่เราต้องการ
npm remove module_name

# แสดงรายการ modules ที่อยู่ในโปรเจกปัจจุบัน (ทั้งหมด)
npm list

# ระบุคำสั่งเพื่อจัดการกับ module ในระดับ global หมายถึง module ที่ติดตั้งไว้ในเครื่องของเรา 
# ไม่ใช่ module ที่ถูกติดตั้งอยู่ในเฉพาะโปรเจกปัจจุบันเท่านั้น
# หรือ module ที่สามารถรันคำสั่งได้เลย โดยไม่ต้องติดตั้งซ้ำ
# ยกตัวอย่าง การใช้งานคำสั่งจัดการกับ module ในระดับ global เช่น

npm install module_name -g # คำสั่งติดตั้ง module
npm update module_name -g # คำสั่งอัพเดท module
npm remove module_name -g # คำสั่งถอนติดตั้ง module
npm list -g # คำสั่งแสดงรายการ modules

# ติดตั้ง module ที่ติดตั้งเพื่อใช้ร่วมกับโปรเจกของเรา และ กรณีมีการ Build ไฟล์ module 
# จะถูกรวมไว้ในไฟล์ Build ของ Production นั่นเอง

npm install module_name --save # คำสั่งติดตั้ง module
npm update module_name --save # คำสั่งอัพเดท module
npm remove module_name --save # คำสั่งถอนติดตั้ง module

# ติดตั้ง module กรณีมีการใช้ในการพัฒนาโปรเจกเท่านั้น และ กรณีมีการ Build ไฟล์ module 
# จะไม่ถูกรวมไว้ในไฟล์ Build ของ Production นั่นเอง

npm install module_name --save-dev # คำสั่งติดตั้ง module
npm update module_name --save-dev # คำสั่งอัพเดท module
npm remove module_name --save-dev # คำสั่งถอนติดตั้ง module
