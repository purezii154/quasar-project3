<template>
  <div class="htmlClass">
    <h1>{{ title }}</h1>
    <form>
      <input type="text" id="firstName" v-model="firstName" />
      <input type="text" id="secondName" v-model="secondName" />
      <button @click="submitForm()" class="submitForm">Submit</button>
  </form>
  </div>
</template>

<script>
export default {
  name: 'InputPage',
  data() {
    return {
      title: 'วิวัฒนาการของโลกสมัยใหม่.',
      nickname: 'เพียว',
      firstName: 'นพดล',
      secondName: 'เพ่งพิศ',
      studentCode : '404',
    }
  },
  methods: {
    submitForm() {
      this.$emit('submit form')
    },
  }
}
</script>

<style scoped></style>
