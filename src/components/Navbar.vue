<template>
  <div class="navbar">
    <div class="left-side" onclick="window.location.hash = '#'">
      <img src="@/assets/logo.svg" alt=""/>
      <h2>YourText</h2>
    </div>
    <nav>
      <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">About</a></li>
        <li><a href="#">Contact</a></li>
      </ul>
    </nav>
  </div>
</template>

<script>
export default {
  name: 'Navbar',
};
</script>

<style scoped>
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1rem;
  background-color: var(--background-color);
  border-bottom: 1px solid var(--border-color);
}

.left-side {
  display: flex;
  align-items: center;
  cursor: pointer;
}

img {
  width: 48px;
}

nav {
  background-color: var(--background-color);
}

ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
  background-color: var(--background-color);
}

li {
  float: left;
}

li a {
  font-size: 20px;
  font-weight: bold;
  display: block;
  color: white;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

li a:hover {
  background-color: var(--text-color);
  color: var(--background-color);
}
</style>
