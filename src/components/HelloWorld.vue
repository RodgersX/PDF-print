<template>
  <div class="hello">
    <div id="printMe">
      <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ducimus maiores perferendis obcaecati ratione tenetur commodi deserunt corrupti iusto. Placeat consequatur suscipit molestias nobis id labore aliquam quo quos eaque libero?</p>
    </div>

    <button @click="print">print</button>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data() {
    return {
      output: null
    }
  },

  methods: {
    print() {
      this.$htmlToPaper('printMe')
    }
  }
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
