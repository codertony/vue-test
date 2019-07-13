<template>
    <div>
        <div v-for="n in list" :key="n">
            {{n}}
        </div>
    </div>
</template>

<script>
  export default {
    name: 'testList',
    props: ['list']
  }
</script>

<style scoped>

</style>
