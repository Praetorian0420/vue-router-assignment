<template>
  <div id="app">
    <nav>
      <RouterLink to="/">Home</RouterLink>
      <RouterLink to="/about">About</RouterLink>
      <RouterLink to="/contact">Contact</RouterLink>
    </nav>

    <RouterView />
  </div>
</template>

<style>
body {
  margin: 0;
  background: linear-gradient(135deg, #eef6ff 0%, #dfefff 100%);
  font-family: Arial, sans-serif;
  color: #1d2a3a;
}

#app {
  max-width: 900px;
  margin: 0 auto;
  padding: 40px 24px 60px;
}

nav {
  display: flex;
  gap: 18px;
  margin-bottom: 28px;
  padding: 16px 20px;
  background-color: #ffffff;
  border-radius: 12px;
  box-shadow: 0 2px 8px rgba(15, 23, 42, 0.08);
}

nav a {
  text-decoration: none;
  color: #244a7a;
  font-weight: 700;
  font-size: 1rem;
  transition: color 0.2s ease;
}

nav a:hover {
  color: #0d3b82;
}

nav a.router-link-active {
  color: #d14f4f;
  border-bottom: 2px solid #d14f4f;
  padding-bottom: 4px;
}

h1 {
  color: #1d3557;
  margin-bottom: 12px;
}

p {
  font-size: 1.05rem;
  line-height: 1.7;
  color: #2c3e50;
}
</style>