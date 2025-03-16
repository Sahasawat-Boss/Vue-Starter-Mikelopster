# V-Model

- สิ่งที่เราทำกันด้านบนเป็น 1 way binding คือ เรา update อะไร เราต้องคอยบอก update ให้กับตัวแปรนั้นด้วย
- Vue ได้เตรียม attribute v-model ที่สามารถผูก value ของตัวแปร Reactive เข้ากับ value ของ input ออกมาได้

## Event
onclick="functionName()" ใน javascript
- มีค่าเทียบเท่ากับ v-on:click="functionName()"
- หรือเทียบเท่ากับ @click="functionName()"