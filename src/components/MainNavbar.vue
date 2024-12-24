<template>
  <div class="header">
    <div class="header-inner">
      <img class="logo" alt="School Logo" src="@/assets/school-logo.jpg" />
      <ul class="nav-list">
        <li>About Us</li>
        <li>Podcast</li>
        <li>Events</li>
        <li>Gallery</li>
        <li>Contact Us</li>
      </ul>
      <button class="join-button">Join The Lounge</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "MainNavbar",
};
</script>

<style scoped>
.header {
  height: auto;
  background-color: #fcfdf2;
  margin-top: -55px;
  padding: 10px 20px;
  border-bottom: 2px solid #e0e0e0;
}

.header-inner {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0 20px;
  max-width: 1200px;
  margin: 0 auto;
}

.logo {
  width: 150px;
  height: auto;
  object-fit: contain;
}

.nav-list {
  display: flex;
  list-style: none;
  padding: 0;
  margin: 0;
  gap: 50px;
}

.nav-list li {
  cursor: pointer;
  font-size: 16px;
  color: #333;
  transition: color 0.3s ease;
}

.nav-list li:hover {
  color: #4a5ae5;
}

.join-button {
  padding: 12px 20px;
  background-color: #4a5ae5;
  color: white;
  border: none;
  border-radius: 5px;
  cursor: pointer;
  font-size: 16px;
  transition: background-color 0.3s ease;
}

.join-button:hover {
  background-color: #4a065d;
}

@media (max-width: 768px) {
  .header-inner {
    flex-direction: column;
    align-items: center;
  }

  .nav-list {
    flex-direction: column;
    gap: 20px;
    margin-top: 15px;
  }

  .join-button {
    margin-top: 10px;
  }
}

@media (max-width: 480px) {
  .logo {
    width: 120px;
  }

  .nav-list li {
    font-size: 14px;
  }

  .join-button {
    font-size: 14px;
    padding: 10px 15px;
  }
}
</style>
