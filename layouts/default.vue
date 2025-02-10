<template>
    <div>
      <nav class="navbar navbar-expand-lg navbar-custom">
        <a class="navbar-brand mx-auto" href="#">Zeynep Tatar</a>
      </nav>
     <main>
     <NuxtPage/>
     </main>
     
      <footer class="footer-custom">
        <div class="container">
          <div class="row">
            <div class="col-6 col-md-3 social-media">
              <a href="https://www.instagram.com" target="_blank">
                <i class="fab fa-instagram"></i>
              </a>
            </div>
            <div class="col-6 col-md-3 social-media">
              <a href="https://www.linkedin.com" target="_blank">
                <i class="fab fa-linkedin"></i>
              </a>
            </div>
            <div class="col-6 col-md-3 social-media">
              <a href="mailto:someone@example.com" target="_blank">
                <i class="fas fa-envelope"></i>
              </a>
            </div>
            <div class="col-6 col-md-3 social-media">
              <a href="https://github.com" target="_blank">
                <i class="fab fa-github"></i>
              </a>
            </div>
          </div>
          <div class="text-center mt-3">
            <p>&copy; 2025 Zeynep Tatar. Tüm hakları saklıdır.</p>
          </div>
        </div>
      </footer>
    </div>
  </template>
  
  <script>
  export default {
    name: 'NavbarComponent'
  }
  </script>
  
  <style scoped>
  @import url('https://fonts.googleapis.com/css2?family=Playfair+Display:wght@700&display=swap'); /* Playfair Display fontunu dahil ettik */
  
  /* Sayfa arka plan rengini değiştiriyoruz */
  body {
    background-color: #210440; /* Koyu mor arka plan */
    margin: 0;
    padding: 0;
    padding-bottom: 150px; /* Footer'ın üstüne gelmemesi için */
  }
  
  /* Navbar için şeftali tonu ve özel stil */
  .navbar-custom {
    background-color: rgba(255, 255, 255, 0);
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    box-shadow: 0 5px 5px rgba(0, 0, 0, 0.1); /* Hafif gölge */
    z-index: 10; /* Navbar'ı önde tutar */
  }
  
  .navbar-custom .navbar-brand {
    color: #874335;
    font-size: 30px;
    font-family: 'Playfair Display', serif;
    text-align: center;
    letter-spacing: 2px;
  }
  
  .navbar-custom .navbar-brand:hover {
    color: #b35947;
  }
  
  /* Footer */
  .footer-custom {
    background-color: rgba(255, 255, 255, 0); /* Navbar ile aynı şeftali rengi */
    padding: 30px 0;
    color: #874335;
    font-family: 'Playfair Display', serif;
    max-height: 100px;
    bottom: 0;
    left: 0;
    width: 100%;
    text-align: center;
    z-index: 1; /* Footer'ı en altta tutar */
    position: fixed;
     
  }
  
  /* Footer iconlar */
  .social-media {
    display: flex;
    justify-content: center;
    align-items: center;
    margin-bottom: 15px;
  }
  
  .social-media a {
    color: #874335;
    font-size: 40px; /* İkonları büyütüyoruz */
    transition: color 0.3s ease;
    margin: 0 10px;
  }
  
  .social-media a:hover {
    color: #874335;
  }
  
  /* Responsive düzenlemeler */
  @media (max-width: 768px) {
    .social-media {
      margin-bottom: 20px;
    }
  }
  </style>
  