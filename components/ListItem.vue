<template functional>
  <div class="list-item-body">
    <h4>
      <a href="https://jsonplaceholder.typicode.com/" target="_blanks">
        {{ props.title.toUpperCase() }}
      </a>
    </h4>
    <section>
      <p>{{ props.body }}</p>
      <a href="http://placecorgi.com/" target="_blank">
        <img src="http://placecorgi.com/360/180"
      /></a>
    </section>
  </div>
</template>

<style scoped>
.list-item-body {
  border: 2px solid #21a179;
  background-color: #eee;
  border-radius: 5px;
  padding: 15px 30px 15px 30px;
  box-shadow: 3px 10px #21a179;
}
a {
  text-decoration: none;
  color: hsl(12, 93%, 40%);
  transition: 0.3s;
}
a:hover {
  color: hsl(12, 93%, 30%);
}
div {
  margin: 10px;
}
h4 {
  font-size: 2rem;
  font-weight: 700;
  text-align: left;
  margin-bottom: 1rem;
  border-bottom: hsl(12, 93%, 40%) 1px solid;
  transition: 0.3s;
}
h4:hover {
  box-shadow: 0px 2px hsl(12, 93%, 40%);
  transform: translateY(-2px);
}

section {
  display: flex;
  justify-content: space-between;
}

p {
  font-size: 1.5rem;
  text-align: justify;
}
img {
  margin: 5px 0 5px 50px;
  border: 5px hsl(12, 93%, 40%) solid;
  box-shadow: 5px 10px hsl(12, 93%, 25%);
  transition: 0.3s;
}
img:hover {
  transform: translate3d(-5px, -10px, 10px);
  box-shadow: 10px 20px hsl(12, 93%, 25%);
}
</style>
