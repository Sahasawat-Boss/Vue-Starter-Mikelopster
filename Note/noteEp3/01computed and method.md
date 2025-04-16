# Computed properties

src: https://docs.mikelopster.dev/c/vue-firebase/chapter-3/computed

computed properties คือการห่อ logic หรือการคำนวนของ data เอาไว้แล้ว return ค่าออกไปเป็น result ตัวใหม่

pain point ของ computed properties คือ เราอาจจะมีโจทย์ที่ต้องการใส่ Logic กับตัวแปรไว้ แต่ไม่ต้องการมาคอยใส่ logic ใน template เช่น

เคสหาความยาวของ Array
เคสเอา string มาต่อกัน เช่น ชื่อ, นามสกุล
เราก็เลยจะใช้ computed มาแก้ปัญหานี้

...

Work with reactive or ref