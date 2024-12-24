<template>
    <section>
      <div class="hero-bg">
        <div class="inner-bg">
          <div class="hero-content">
            <h1>Thinking of Running Away?</h1>
            <p>
              We get it. Home doesn’t always feel like home. But before you make any big decisions,
              there’s a better way—and we’re here to help you find it.
            </p>
            <button>Let’s Figure This Out Together</button>
            <img src="@/assets/school-logo.jpg" alt="">

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
    background-color: #fcfdf2;
    height: 90vh;
    display: flex;
    align-items: center;
    justify-content: center;
    margin-top: -10px;
    padding: 0 20px;
  }
  
  .inner-bg {
    background-color: #4a5ae5;
    height: 70vh;
    width: 100%;
    max-width: 1200px;
    display: flex;
    align-items: center;
    justify-content: center;
    border-radius: 20px;
    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
    margin-top: -30px;
    padding: 40px; 
    text-align: center;
  }
  
  .hero-content {
    color: white;
    max-width: 700px;
    text-align: center;
  }
  
  .hero-content h1 {
    font-size: 3rem;
    margin-bottom: 20px;
    line-height: 1.2;
  }
  
  .hero-content p {
    font-size: 1.2rem;
    margin-bottom: 30px;
    line-height: 1.6;
    word-wrap: break-word;
  }
  
  .hero-content button {
    padding: 15px 30px;
    background-color: #fcfdf2;
    color: #4a5ae5;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    font-size: 1rem;
    font-weight: bold;
    transition: background-color 0.3s, color 0.3s;
  }
  
  .hero-content button:hover {
    background-color: #4a5ae5;
    color: #fcfdf2;
  }
  
  @media (max-width: 768px) {
    .inner-bg {
      height: 60vh;
      width: 90%;
      border-radius: 15px;
    }
  
    .hero-content h1 {
      font-size: 2.5rem;
    }
  
    .hero-content p {
      font-size: 1rem;
    }
  
    .hero-content button {
      font-size: 0.9rem;
      padding: 10px 20px;
    }
  }
  
  @media (max-width: 480px) {
    .inner-bg {
      height: 50vh;
    }
  
    .hero-content h1 {
      font-size: 2rem;
    }
  
    .hero-content p {
      font-size: 0.9rem;
    }
  
    .hero-content button {
      font-size: 0.8rem;
      padding: 8px 16px;
    }
  }
  </style>
  