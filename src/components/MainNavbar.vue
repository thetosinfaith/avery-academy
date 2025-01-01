<template>
  <div class="header">
    <div class="header-inner">
      <img class="logo" alt="School Logo" src="@/assets/muve.png" />
      <div class="hamburger" @click="toggleNav">
        <span></span>
        <span></span>
        <span></span>
      </div>
      <ul class="nav-list" :class="{ 'show': isNavVisible }">
        <li>About Us</li>
        <li>Stories</li>
        <li>Events</li>
        <li>Merch</li>
        <li>Contact Us</li>
        <li class="mobile-join-button">
          <button class="join-button">I’m Ready to Muve</button>
        </li>
      </ul>
      <button class="join-button desktop-join-button">I’m Ready to Muve</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "MainNavbar",
  data() {
    return {
      isNavVisible: false,
    };
  },
  methods: {
    toggleNav() {
      this.isNavVisible = !this.isNavVisible;
    },
  },
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
  max-width: 1100px;
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
  transition: all 0.3s ease;
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
  font-size: 1.2rem;
  transition: background-color 0.3s ease;
  font-family: "Outfit", serif;
}

.join-button:hover {
  background-color: #4a065d;
}

.hamburger {
  display: none;
  cursor: pointer;
  flex-direction: column;
  gap: 5px;
  justify-content: space-between;
  height: 30px;
}

.hamburger span {
  width: 30px;
  height: 5px;
  background-color: #333;
  transition: all 0.3s ease;
}

.desktop-join-button {
  display: none;
}

@media (max-width: 768px) {
  .header-inner {
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
    width: 100%;
  }

  .nav-list {
    flex-direction: column;
    gap: 20px;
    margin-top: 15px;
    display: none;
  }

  .desktop-join-button {
    display: none;
  }

  .hamburger {
    display: flex;
  }

  .nav-list.show {
    display: flex;
  }

  .mobile-join-button {
    display: block;
    text-align: center;
  }

  .join-button {
    display: none;
  }
}

@media (max-width: 480px) {
  .logo {
    width: 60px;
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
