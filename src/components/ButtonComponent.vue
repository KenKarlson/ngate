<template>
  <div>
    <h2>Button</h2>

    <div class="mb-3">
      <button @click="count--" class="mr-1">Dec-</button>
      <button @click="count++" class="mr-1">Inc+</button>
      <button @click="resetCount(0)" class="mr-1">Reset</button>
      <span>{{countValue}}</span>
    </div>
  </div>
</template>
<script>
export default{
  data(){
    return {
      count:0
    }
  },
  computed: {
    countValue(){
      return "Текущее значение: "+this.count;
    }
  },
  methods:{
    resetCount(value){
      return this.count = value;
    }
  }
}
</script>