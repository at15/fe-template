<template>
    <div>
        <p> example: sql
        </p>
        <textarea cols="30" rows="10" placeholder="enter SQL" v-model="sql">
  </textarea>
        <button v-on:click="query">query</button>
        <textarea cols="30" rows="10" v-model="result" readonly placeholder="result"></textarea>
    </div>
</template>

<script>
import alasql from 'alasql';

export default {
  data () {
    alasql('CREATE TABLE example1 (a INT, b INT)');
    alasql.tables.example1.data = [
      // Insert data directly from JavaScript object...
      { a: 2, b: 6 },
      { a: 3, b: 4 }
    ];
    const sql = 'SELECT * from example1';
    return {
      sql: sql,
      result: ''
    };
  },
  methods: {
    query: function (event) {
      if (this.sql === '') {
        console.warn('empty sql');
        return;
      }
      try {
        const res = alasql(this.sql);
        console.log(res);
        this.result = JSON.stringify(res);
      } catch (e) {
        // TODO: need to display the error
        console.warn(e);
      }
    }
  }
};
</script>
