<template>
  <header>
    <nav>
      <ul>
        <li><a href="#">Domov</a></li>
        <li><a href="#">Produkty</a></li>
        <li><a href="#">Kontakt</a></li>
      </ul>
    </nav>

    <div class="hero">
      <video autoplay muted loop>
        <source src="@/assets/lava.mp4" type="video/mp4" />
        Váš prehliadač nepodporuje video tag.
      </video>
      <div class="overlay">
        <h1>Vitajte na našom e-shope</h1>
        <p>Najlepšie produkty za skvelé ceny len pre vás.</p>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style scoped>
header {
  position: relative;
  width: 100%;
  height: 100vh;
  overflow: hidden;
}

nav {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  background: rgba(0, 0, 0, 0.7);
  padding: 1rem 0;
  text-align: center;
}

nav ul {
  list-style: none;
  padding: 0;
  margin: 0;
  display: flex;
  justify-content: center;
  gap: 20px;
}

nav ul li {
  display: inline;
}

nav ul li a {
  color: white;
  text-decoration: none;
  font-size: 1.2rem;
  font-weight: bold;
}

.hero {
  position: relative;
  width: 100%;
  height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
}

.hero video {
  position: absolute;
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.overlay {
  position: absolute;
  text-align: center;
  color: white;
  background: rgba(0, 0, 0, 0.5);
  padding: 20px;
  border-radius: 10px;
}

.overlay h1 {
  font-size: 3rem;
  margin-bottom: 10px;
}

.overlay p {
  font-size: 1.2rem;
}
</style>
