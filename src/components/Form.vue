<script setup>
import { reactive } from "vue"

let formData = reactive({
  firstname: "",
  lastname: "",
  age: "",
  gender: "",
  interests: [],
  description: "",
})

const gendersList = ['ชาย', 'หญิง', 'ไม่ระบุ']
// v-for="gender in gendersList" v-bind:key="gender"
const interestsList = ['หนังสือ', 'กีฬา', 'การเมือง', 'game']
// v-for="interest in interestsList" v-bind:key="interest"

const submitData = () => {
  console.log('formData', JSON.parse(JSON.stringify(formData)))
  console.log('interest', formData.interests.join())
}
</script>

<template>
  <div>
    <div>
      <div>ชื่อจริง</div>
      <input class="form" type="text" v-model="formData.firstname" />
    </div>
    <div>
      <div>นามสกุล</div>
      <input class="form" type="text" v-model="formData.lastname" />
    </div>
    <div>
      <div>อายุ</div>
      <input type="number" min="0" max="100" v-model="formData.age" />
    </div>
    <div>
      <div>เพศ</div>
      <div v-for="gender in gendersList" v-bind:key="gender">
        <input type="radio" :value="gender" v-model="formData.gender"> {{ gender }}
      </div>
    </div>
    <div>
      <div>สิ่งที่สนใจ</div>
      <div v-for="interest in interestsList" v-bind:key="interest">
        <input type="checkbox" :value="interest" v-model="formData.interests"> {{ interest }}
      </div>
    </div>
    <div>
      <div>คำอธิบายเพิ่มเติม</div>
      <textarea></textarea>
    </div>
    <button @click="submitData()">ส่งข้อมูล</button>
  </div>
</template>