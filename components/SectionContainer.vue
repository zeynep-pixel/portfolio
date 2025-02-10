<template>
    <div class="container">
      <div class="row">
        <div class="section">
           
        </div>
        <div class="section">
           
        </div>
      </div>
      <div class="row">
        <div class="section">
           
        </div>
        <div class="section">
           
        </div>
        
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'ResponsiveGrid',
  }
  </script>
  
  <style scoped>
  @import url('https://fonts.googleapis.com/css2?family=Playfair+Display:wght@700&display=swap');
  /* Sayfa içeriğini dolduracak şekilde */
  .container {
    margin-top: 80px;
    margin-bottom: 80px;
    display: flex;
    flex-direction: column; /* Başlangıçta dikey düzen */
    height: 100vh; /* Sayfanın tamamını kapsayacak şekilde */
  }
  
  .row {
    display: flex;
    justify-content: space-between; /* Hücreler arasında boşluk bırak */
    flex: 1; /* Her satır eşit yer kaplasın */
  }
  
  .section {
    flex: 1;
    margin: 10px;
    background-color: #fffcfc2d; 
    display: flex;
    justify-content: center;
    align-items: center;
    border-radius: 10px;
    font-family: 'Playfair Display';
    font-size: 20px;
    color: white;
    letter-spacing: 2px;
  }
  
  @media (max-width: 500px) {
    /* Ekran küçükse, öğeleri alt alta getirmek için */
    .row {
      flex-direction: column; /* Dikey hizalamayı sağla */
    }
  
    .section {
      margin: 5px 0;
       /* Bölümler arasındaki boşluğu azalt */
    }
  }
  
  @media (max-width: 480px) {
    .section p {
      font-size: 14px; /* Yazıyı küçült */
    }
  }
  </style>
  