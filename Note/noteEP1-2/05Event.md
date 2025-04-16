## Event
https://docs.mikelopster.dev/c/vue-firebase/chapter-2/event

- onclick="functionName()" ใน javascript
- มีค่าเทียบเท่ากับ v-on:click="functionName()"
- หรือเทียบเท่ากับ @click="functionName()"

ซึงวิธีการ binding event มีทั้งหมด 2 ประเภทคือ

- Inline handler = การใส่ inline javascript เพื่อเพิ่ม function ให้ trigger event
- Method handler = เป็นการระบุ property หรือ path ที่ชี้สู่ method ใน Component ของ Event