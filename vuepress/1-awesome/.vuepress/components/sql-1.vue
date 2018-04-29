<template>
<div>
  I want some sql
  <textarea cols="30" rows="10" placeholder="enter SQL" v-model="sql">
  </textarea>
  <button v-on:click="query">query</button>
</div>
</template>

<script>
import alasql from "alasql";

export default {
  data() {
    alasql("CREATE TABLE example1 (a INT, b INT)");
    alasql.tables.example1.data = [
      // Insert data directly from JavaScript object...
      { a: 2, b: 6 },
      { a: 3, b: 4 }
    ];
    let sql = "SELECT * from example1";
    return {
      sql: sql
    };
  },
  methods: {
    query: function(event) {
      if (this.sql === "") {
        console.warn("empty sql");
        return;
      }
      let res = alasql(this.sql);
      console.log(res);
    }
  }
};
</script>
