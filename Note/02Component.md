## Component 

คือ 1 ใน core concept ของ vue. Component คือการแบ่งส่วนเว็บออกเป็นชิ้นเล็กๆทีรวม 
html, css และ javascript เอาไว้ในก้อนเดียวกัน นั่นคือ

1. template (html)
2. script (javascript logic)
3. style (css styling)

## Main js

- Import Conponent หลักออกมาแล้วเอามาสร้างเป็น Application
- Mount กลับมาที่ Html ตาม id (#app)

# Browser อ่าน .Vue ไม่ได้ Vite แปลงให้เป็น HTML CSS JS
ต้องถูก แปลง (compile) เป็น HTML, CSS และ JavaScript ก่อนที่ browser จะสามารถรันได้

เมื่อคุณใช้ Vite (npm run dev), มันจะ:
- Compile ไฟล์ .vue → เป็น JavaScript module (.js)
- แยก CSS ออกมา → ทำให้โหลดเร็วขึ้น
- Bundle ทุกอย่างให้ browser ใช้งานได้ โดยใช้ ES Module (import/export)