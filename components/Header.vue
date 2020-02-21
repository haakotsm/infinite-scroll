<template>
  <header>
    <img src="../assets/logo.svg" />
    <ul class="header-list">
      <li>
        <a href="http://www.vg.no" target="_blank" rel="noopener noreferrer">
          VG
        </a>
      </li>
      <li>
        <a
          href="http://www.aftenposten.no"
          target="_blank"
          rel="noopener noreferrer"
        >
          Aftenposten
        </a>
      </li>
      <li>
        <a
          href="http://www.dagbladet.no"
          target="_blank"
          rel="noopener noreferrer"
        >
          Dagbladet
        </a>
      </li>
    </ul>
  </header>
</template>

<script>
export default {};
</script>

<style scoped>
header {
  top: 0;
  position: fixed;
  width: 100vw;
  min-height: 50px;
  display: flex;
  background-color: #c4af9a;
  box-shadow: 0px 5px hsl(30, 26%, 63%);
  padding: 0 20px 0 20px;
}

.header-list {
  flex-grow: 1;
  list-style: none;
  display: flex;
  justify-content: space-around;
  align-items: center;
}
.header-list > li > a {
  font-weight: 700;
  text-decoration: none;
  color: #1e1e24;
}
</style>
