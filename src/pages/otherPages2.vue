<template>
  <div class="container">

    <ol>
      <li
        v-for="(item, index) in arr"
        @click='test(item.text)'
      >
        {{index}}: {{item.text}}
      </li>
    </ol>

  </div>
</template>









<script>
import component22 from "./component22";

export default {
  data() {
    return {
      arr: []
    };
  },
  created() {
    this.loadList();
  },
  methods: {
    loadList: function(text) {
      const list = [
        {
          text: 1
        },
        {
          text: 2
        },
        {
          text: 3
        }
      ];

      this.arr = list;
    }
  }
};
</script>













<style scoped>
.parent-tit {
  margin-top: 30px;
}
h4 {
  font-size: 20px;
}
h2 {
  margin: 0 0 40px;
}
.text-center p {
  color: #41b883;
}
</style>
