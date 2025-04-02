# Data Binding

## รู้จักกับ Reactive ก่อนว่าคืออะไร ?
- Vue นั้นมีความสามารถ track change ของ state และ สามารถ update DOM 
- เมื่อมี change เกิดขึ้นได้แบบ automatically โดยที่เราไม่ต้องคอยใช้คำสั่งอย่าง .innerHTML หรือคอย update ตัวแปรกลับได้

- ซึ่งคุณสมบัตินี้เราเรียกกันว่า Reactive คือความสามารถในการจัดการกับ view ใน DOM ได้อย่างอัตโนมัติ 
- ซึ่งนี้เป็นข้อดีอย่างมากในการพัฒนา Frontend มันจะช่วยประหยัดทั้งคำสั่งของ javascript และอำนวยความสะดวกในการจัดการ state ของ javascript ด้วย

## รู้จักกับ Ref
- ท่าแรกสำหรับทำ reactive ของ Composition API คือ ref()

- ref() คือคำสั่งที่เปลี่ยนตัวแปรที่รับให้กลายเป็นตัวแปรแบบ reactive
argument ที่ใส่ใน ref() คือค่าเริ่มต้นของตัวแปร และ .value คือวิธีดึงค่าและ update กลับไปผ่านตัวแปร reactive ได้

## รู้จักกับ Reactive
- ใช้กับเคสที่เป็น object สามารถแปลง object ออกมาได้เลย 
(ถ้าใช้ ref() มันจะต้อง .value เสมอ แต่ถ้าใช้ reactive() จะดึง object ออกมาได้เลย)

Reactive > Ref make it easier


## แนะนำ
ทั้วไปใช้ Ref

Object ใหญ่ๆใช้ Reative