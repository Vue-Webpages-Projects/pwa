<template>
  <div>
    <b-container>
      <!-- <b-row>
        <b-col sm="12" md="4">
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Molestias quia voluptatem excepturi odit quae debitis in tempora modi ipsam sunt, dolor nisi veniam eaque? Veritatis illo nostrum, autem culpa ab quia. Ipsum sunt reprehenderit nobis harum itaque ea quos natus beatae, ut ipsa voluptatibus atque unde perferendis debitis repellendus distinctio?
          </p>
        </b-col>
        <b-col sm="12" md="4">
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Molestias quia voluptatem excepturi odit quae debitis in tempora modi ipsam sunt, dolor nisi veniam eaque? Veritatis illo nostrum, autem culpa ab quia. Ipsum sunt reprehenderit nobis harum itaque ea quos natus beatae, ut ipsa voluptatibus atque unde perferendis debitis repellendus distinctio?
          </p>
        </b-col>
        <b-col sm="12" md="4">
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Molestias quia voluptatem excepturi odit quae debitis in tempora modi ipsam sunt, dolor nisi veniam eaque? Veritatis illo nostrum, autem culpa ab quia. Ipsum sunt reprehenderit nobis harum itaque ea quos natus beatae, ut ipsa voluptatibus atque unde perferendis debitis repellendus distinctio?
          </p>
        </b-col>
      </b-row> -->
    </b-container>

    <group />

    <div style="height: 1000px"></div>

  </div>
</template>

<script>

import Group from './Group.vue'

export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  components: {
    Group
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
