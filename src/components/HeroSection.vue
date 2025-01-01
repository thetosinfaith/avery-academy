<template>
  <section>
    <div class="hero-bg">
      <div class="hero-layout">
        <div class="hero-image">
          <img src="@/assets/roam.png" alt="Hero Image" />
        </div>
        <div class="hero-content">
          <h1>Your Next Big Move Starts Here!</h1>
          <p>
            Muve is for anyone ready to leave home and live independently. It’s a collaborative effort between us & you to provide the support to help you build the future you’ve always dreamed of.
          </p>
          <div class="button-group">
            <button aria-label="Start the journey">Get Support</button>
            <button aria-label="partner">Partner With Us</button>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "HeroSection",
};
</script>

<style scoped>
.hero-bg {
  height: 85vh;
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 0 20px;
  background-color: #5873FE;
}

.hero-layout {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-wrap: wrap;
  max-width: 1500px;
  width: 100%;
  gap: 40px;
}

.hero-image {
  flex: 1;
  max-width: 500px;
  display: flex;
  align-items: center;
  justify-content: center;
}

.hero-image img {
  width: 85%;
  height: 500px;
  border-radius: 10px;
  border: 4px dashed white;
}

.hero-content {
  flex: 1;
  max-width: 600px;
  text-align: left;
  font-family: "Outfit", sans-serif;
  margin-bottom: 5%;
}

.hero-content h1 {
  font-size: 4.5rem;
  margin-bottom: 1.5rem;
  line-height: 1.4;
  color: white;
}

.hero-content p {
  font-size: 1.2rem;
  margin-bottom: 2.5rem;
  line-height: 1.8;
  color: white;
}

.button-group {
  display: flex;
  gap: 1.5rem;
}

.button-group button:first-child {
  background-color: white;
  color: #5873FE;
}

.button-group button:last-child {
  background-color: #5873FE;
  color: white;
  border: 1px solid white;
}

.hero-content button {
  padding: 15px 20px;
  background-color: white;
  color: #5873FE;
  border: none;
  border-radius: 5px;
  cursor: pointer;
  font-size: 1.2rem;
  font-weight: 600;
  transition: transform 0.3s, box-shadow 0.3s;
  font-family: "Outfit", sans-serif;
}

.hero-content button:hover {
  transform: translateY(-2px);
  box-shadow: 0 5px 15px rgba(74, 90, 229, 0.3);
}

@media (max-width: 768px) {

  .hero-bg {
  height: auto;
}

  .hero-layout {
    flex-direction: column;
    text-align: center;
  }

  .hero-content h1 {
    font-size: 2.5rem;

  }

  .hero-content p {
    font-size: 1rem;
    font-family: "Outfit", sans-serif;

  }

  .button-group {
    flex-direction: column;
    gap: 10px;
  }

  .hero-content button {
    width: 100%;
  }
}

@media (max-width: 480px) {
  .hero-bg {
    height: 120vh;
    display: flex; 
    flex-direction: column; 
  }

  .hero-content {
    order: 1; 
    margin-top: 10%;
  }

  .hero-image {
    order: 2; 
  }

  .hero-image img {
    order: 2; 
    margin-bottom: 10%;
  }


  .hero-content h1 {
    font-size: 2rem;
    font-family: "Outfit", sans-serif;
  }

  .hero-content p {
    font-size: 0.9rem;
    font-family: "Outfit", sans-serif;
  }

  .hero-content button {
    font-size: 0.9rem;
    padding: 10px 20px;
  }

  .hero-image img {
    height: 400px;
    width: 100%;
  }
}
</style>
