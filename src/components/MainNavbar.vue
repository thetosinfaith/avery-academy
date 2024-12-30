<template>
  <div class="header">
    <div class="header-inner">
      <img class="logo" alt="School Logo" src="@/assets/muve.png" />
      <ul class="nav-list">
        <li>About Us</li>
        <li>Stories</li>
        <li>Events</li>
        <li>Merch</li>
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
  width: 100px;
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
  font-size: 18px;
  color: #333;
  transition: color 0.3s ease;
  font-family: "Outfit", serif;
}

.nav-list li:hover {
  color: #5873FE;
}

.join-button {
  padding: 15px 20px;
  background-color: #5873FE;
  color: white;
  border: none;
  border-radius: 5px;
  cursor: pointer;
  font-size: 16px;
  transition: background-color 0.3s ease;
  font-family: "Outfit", serif;
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
