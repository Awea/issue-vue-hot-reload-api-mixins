<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <p>{{ internalData }}</p>
  </div>
</template>

<script>
export default {
  data(){
    return {
      internalData: ''
    }
  },
  props: {
    msg: String
  },
  methods: {
    // Try comment/uncomment this and see the data disapear from HelloWorld.vue
    foo(){
      console.log('bar')
    }
  }
}
</script>