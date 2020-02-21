<template functional>
  <div class="list-item-body">
    <h4>{{ props.title }}</h4>
    <p>{{ props.body }}</p>
  </div>
</template>

<style scoped>
.list-item-body {
  border: 2px solid #21a179;
  background-color: #eee;
  border-radius: 5px;
  padding: 5px 15px 5px 15px;
  box-shadow: 3px 10px #21a179;
}
div {
  margin: 10px;
}
h4 {
  font-size: 1.5rem;
  font-weight: 700;
  color: #fb9f89;
  text-align: left;
}
p {
  font-size: 1.2rem;
}
</style>
