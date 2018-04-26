<template>
<div>
  <p>
      I am {{ foo }}
  </p>
  awesome databases
  <table>
      <thead>
          <tr>
              <th>Name</th>
              <th>Language</th>
              <th>Backend</th>
          </tr>
      </thead>
      <tbody>
          <tr v-for="db in databases">
            <td>{{ db.name }}</td>
            <td>{{ db.lang }}</td>
            <td>{{ db.backend }}</td>
          </tr>
      </tbody>
  </table>
</div>
</template>

<script>
import { databases } from "../../data/databases";

export default {
  data() {
    console.log(databases);
    return {
      foo: "This is foo",
      databases: databases
    };
  }
};
</script>

