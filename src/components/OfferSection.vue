<template>
    <div class="container">
      <h1 class="main-title">How It Works?</h1>
      <div class="circle-body">
        <div class="circle-item">
          <div class="circle">
            <img src="@/assets/ao.jpg" alt="Image 1">
          </div>
          <h4 class="circle-title">Start with a Plan</h4>
          <p class="circle-subtitle">We’ll chat about what you want, what’s holding you back, and how we can make it work.
</p>
          <a href="#" class="circle-cta">Learn More</a>
        </div>
        <div class="circle-item">
          <div class="circle">
            <img src="@/assets/2.png" alt="Image 2">
          </div>
          <h4 class="circle-title">Learn & Earn</h4>
          <p class="circle-subtitle">Budgeting? Etc? We’ll teach you the stuff no one tells you but everyone needs to know.</p>
          <a href="#" class="circle-cta">Learn More</a>
        </div>
        <div class="circle-item">
          <div class="circle">
            <img src="@/assets/b.png" alt="Image 3">
          </div>
          <h4 class="circle-title">Join the Squad</h4>
          <p class="circle-subtitle">You’re not alone in this. Meet with people who get it and are on the same journey as you.</p>
          <a href="#" class="circle-cta">Learn More</a>
        </div>
        <div class="circle-item">
          <div class="circle">
            <img src="@/assets/m.png" alt="Image 4">
          </div>
          <h4 class="circle-title">Make the Move</h4>
          <p class="circle-subtitle">When you’re ready, we’ll help you transition and stay connected for support.</p>
          <a href="#" class="circle-cta">Learn More</a>
        </div>
      </div>
    </div>
  </template>

  <style scoped>
  .container {
  text-align: center;
  margin: 20px;
  margin-top: 7%;
}

.main-title {
  font-size: 2.5rem;
  margin-bottom: 70px;
}

.circle-body {
  display: flex;
  justify-content: center;
  gap: 5rem; 
}

.circle-item {
  text-align: center;
  width: 200px;

}

.circle {
  width: 200px;
  height: 150px;
  border-radius: 50%;
  overflow: hidden;
  margin: 0 auto 10px auto;
  border: 2px dashed #5873FE;
  margin-bottom: 10%;
}

.circle img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.circle-title {
  font-size: 1.2rem;
  margin: 10px 0;
  font-family: "Outfit", sans-serif;

}

.circle-subtitle {
  font-size: 0.9rem;
  color: #555;
  font-family: "Outfit", sans-serif;

}

.circle-cta {
  display: inline-block;
  margin-top: 10px;
  font-size: 0.9rem;
  color: #5873FE;
  text-decoration: none;
  font-weight: bold;
}

.circle-cta:hover {
  text-decoration: underline;
}

@media (max-width: 768px) {
  .circle-body {
    flex-direction: column;
    gap: 2rem;
  }

  .circle-item {
    width: 100%;
    max-width: 300px;
    margin: 0 auto;
  }

  .main-title {
    font-size: 2rem;
    margin-bottom: 50px;
  }

  .circle {
    width: 150px;
    height: 100px;
  }

  .circle-title {
    font-size: 1rem;
  }

  .circle-subtitle {
    font-size: 0.9rem;
    max-width: 900px;
  }

  .circle-cta {
    font-size: 0.8rem;
  }
}
  </style>
