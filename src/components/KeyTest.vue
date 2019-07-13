<template>
<div>
    <button @click="list=list1">切换1</button>
    <button @click="list=list2">切换2</button>
    <TestList :list="list"/>
    {{test}}
</div>
</template>
<script>
    import TestList from './TestList'
  export default {
    name: 'key-test',
    data(){
      return {
        list: [],
        list1: [1,2,1],
        list2: [2,2],
      }
    },
    props: ['test'],
    components: {
      TestList
    },
    mounted() {
      this.list = this.list1
    }
  }
</script>
