# ใน Vue จะมีการเขียน Code 2 styles อยู่คือ Option API และ Composition API 

## Option API (ท่าที่ใช้มาแต่เดิมของ Vue 2) 

- Pattern ต้องเป็นแบบนี้เสมอเปลี่ยนไม่ได้ 

- ข้อพิจารณา คือ ส่วน code ระหว่าง data และ method แยกกัน หากจัดการ code ไม่ดีส่วน code จะงงมากและ method อาจจะอยู่ผสมๆกันได้ 

 

## Composition API (ท่าที่เพิ่มมาใหม่ของ Vue 3)

- ข้อดี คือ code จะอิสระกว่า สามารถจัดการ code ได้ตามใจชอบกว่า 

- ข้อพิจารณา คือ สำหรับมือใหม่ ที่ยังคิด pattern code ไม่ออก อาจจะงงได้ว่า ส่วนไหนควรเพิ่มไว้ตรงไหนได้ (ไม่ได้มี Guideline เป๊ะๆอย่าง Option API) 

 

Convert Code Style ได้ 