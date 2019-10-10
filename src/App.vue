<template>
  <main id="app">
    <header class="header">
      <h1>Book stacks</h1>
      <nav class="navigation-menu">
        <a href="https://www.badrchoubai.dev/">About</a>
        <a href="https://github.com/BadrChoubai/BookStacks">GitHub</a>
      </nav>
    </header>
    <div class="container">
      <section id="book-stack-start">
        <h2>Book Stack Start</h2>
      </section>
      <section id="book-stack-current">
        <h2>Current Book</h2>
      </section>
      <section id="book-stack-finish">
        <h2>Book Stack Finish</h2>
      </section>
    </div>
  </main>
</template>

<script>
export default {
  name: "app"
};
</script>

<style lang="scss">
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

a {
  text-decoration: none;
  color: #333;
}

.header {
  display: flex;
  justify-content: space-around;
  align-items: center;
}

.navigation-menu {
  display: flex;
  justify-content: space-around;
  width: 150px;

  a {
    background: darken($color: #fff, $amount: 4);
    padding: 16px;
    margin: 4px;
  }
}

.container {
  position: absolute;
  bottom: 0;
  width: 98vw;

  background: lightblue;
  display: flex;
  justify-content: space-around;
  height: auto;
}

@media screen and (max-width: 700px) {
  .container {
    flex-direction: column;
  }
}
</style>
