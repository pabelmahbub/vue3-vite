<template>
  <h1>{{ msg }}</h1>
  <button @click="count++">count is: {{ count }}</button>

  <li style="background-color: pink;" v-for="item in items.slice(0,6)" :key="item">
    {{ item.message }}
</li>

<li style="background-color: red;" v-for="item1 in items.slice(6)" :key="item1">
    {{ item1.message }}
</li>

  <p>E3dit <code>components/HelloWorld.vue</code> to test hot module replacement.</p>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
   
  


  data() {
    return {
      count: 9,
      items: [
      { id:1,message: '111' }, 
      { id:2,message: '2222' },
      { id:3,message: '3333' }, 
      { id:4,message: '4444' },
      { id:5,message: '55555' }, 
      { id:6,message: '6666' },
      { id:7,message: '777oo' }, 
      { id:8,message: '888Bar' }
    ]
    }
  }
}
</script>
