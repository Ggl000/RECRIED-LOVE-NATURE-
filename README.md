# RECRIED-LOVE-NATURE-
!-- Created by Angel Sharma 🧚‍♀️ -->
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Magic Stick Animation nature</title>
<link rel="stylesheet" href="styles.css">
</head>
<body>
  <h1 class="a">Love the nature</h1>
  <div class="container">
  <div class="heart and nature">❤️🌳</div>
  <div class="stick"></div>
  </div>
  <div class="sparkles"></div>

  <script>
      document.querySelector('.stick').addEventListener('click', () => {
  const sparklesContainer = document.querySelector('.sparkles');
  sparklesContainer.innerHTML = ''; // Clear previous sparkles
    
  for (let i = 0; i < 70; i++) {
    const sparkle = document.createElement('div');
    sparkle.classList.add('sparkle');
    const x = Math.random() * 300 - 150;
    const y = Math.random() * 300 - 150;
    sparkle.style.right = `${x}px`;
    sparkle.style.bottom = `${y}px`;
    
    sparkle.style.animation = `sparkleEffect 1s ${Math.random()}s ease-out`;
    sparklesContainer.appendChild(sparkle);
   
    const r = Math.floor(Math.random() * 256);
    const g = Math.floor(Math.random() * 256);
    const b = Math.floor(Math.random() * 256);
     
    sparkle.style.backgroundColor = `rgb(${r}, ${g}, ${b})`;
    
  }
});
  </script>
</body>
</html>
