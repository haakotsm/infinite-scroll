<template>
  <div>
    <ul id="list">
      <li v-for="item in items" :key="item.id" class="list-item">
        <list-item v-bind="item" />
      </li>
      <li>
        <observer v-bind="options" @intersect="intersected" />
      </li>
    </ul>
  </div>
</template>

<script>
import ListItem from "./ListItem";
import Observer from "./Observer";
export default {
  components: {
    ListItem,
    Observer
  },
  data() {
    return {
      page: 1,
      items: [],
      options: {}
    };
  },
  methods: {
    async intersected() {
      const res = await fetch(
        `https://jsonplaceholder.typicode.com/posts?_page=${this.page}&_limit=50`
      );
      // eslint-disable-next-line
      console.log(res);
      this.page++;
      const items = await res.json();
      // eslint-disable-next-line
      console.log(items);
      this.items = [...this.items, ...items];
    }
  }
};
</script>

<style scoped>
#list {
  width: 960px;
  padding: 0.1rem;
  list-style: none;
}
.list-item {
  padding: 0.3rem;
  border: 1 #232323 solid;
}
</style>
