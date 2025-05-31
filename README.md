# CharityWater
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>charity: water - Landing Page</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <div class="yellow-border left"></div>
  <div class="yellow-border right"></div>
  <div class="container">
    <div class="image-bg">
      <!-- Replace the src below with your actual image path -->
      <img src="child-water.jpg" alt="Child catching clean water in hands">
      <div class="content">
        <div class="logo">
          <img src="charity-water-logo.png" alt="charity: water logo">
        </div>
        <div class="headline">
          <h1>Small Drops Together<br>Become a Life-Giving Stream</h1>
          <p class="supporting">
            When you give, you do more than provide water—you give time back to families, open doors to education, protect health, and spark opportunity for generations.<br>
            It starts with you.
          </p>
          <p class="cta">
            <span class="water-emoji">💧</span> Be the drop. Give clean water.
          </p>
        </div>
      </div>
    </div>
  </div>
</body>
</html>
body {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Segoe UI', Arial, sans-serif;
  background: #fff;
  min-height: 100vh;
  overflow-x: hidden;
  position: relative;
}

.yellow-border {
  position: fixed;
  top: 0;
  width: 60px;
  height: 100vh;
  background: #ffd100;
  z-index: 1;
}

.yellow-border.left {
  left: 0;
}

.yellow-border.right {
  right: 0;
}

.container {
  position: relative;
  margin: 0 60px;
  min-height: 100vh;
  display: flex;
  align-items: stretch;
  justify-content: center;
  z-index: 2;
}

.image-bg {
  position: relative;
  flex: 1;
  display: flex;
  align-items: center;
  justify-content: center;
}

.image-bg img {
  width: 100vw;
  height: 100vh;
  object-fit: cover;
  object-position: center;
  display: block;
  position: absolute;
  top: 0;
  left: 0;
  z-index: 0;
}

.content {
  position: relative;
  z-index: 3;
  width: 100%;
  max-width: 600px;
  margin-left: auto;
  margin-right: 100px;
  background: rgba(255,255,255,0); /* transparent for overlay effect */
  display: flex;
  flex-direction: column;
  align-items: flex-end;
}

.logo {
  background: #fff;
  padding: 22px 40px;
  border-radius: 4px;
  margin-bottom: 40px;
  box-shadow: 0 2px 24px rgba(0,0,0,0.04);
  align-self: flex-end;
}

.logo img {
  height: 48px;
  display: block;
}

.headline {
  background: rgba(255,255,255,0.85);
  border-radius: 8px;
  padding: 36px 38px 28px 38px;
  box-shadow: 0 2px 24px rgba(0,0,0,0.03);
  text-align: left;
  max-width: 450px;
}

.headline h1 {
  font-size: 2rem;
  font-weight: 500;
  margin: 0 0 20px 0;
  color: #222;
  line-height: 1.2;
}

.headline .supporting {
  font-size: 1.08rem;
  color: #222;
  margin-bottom: 18px;
  font-weight: 400;
  line-height: 1.5;
}

.headline .cta {
  font-size: 1.06rem;
  color: #0073e6;
  font-weight: 500;
  margin: 0;
}

.water-emoji {
  font-size: 1.16em;
  vertical-align: middle;
  margin-right: 4px;
}

/* Responsive Styles */
@media (max-width: 900px) {
  .container {
    margin: 0 20px;
  }
  .content {
    margin-right: 0;
    align-items: flex-end;
  }
  .headline, .logo {
    max-width: 100%;
    padding: 24px 18px;
  }
}
@media (max-width: 600px) {
  .yellow-border {
    display: none;
  }
  .container {
    margin: 0;
  }
  .headline, .logo {
    padding: 12px 8px;
  }
  .content {
    align-items: center;
    margin: 0;
  }
  .headline h1 {
    font-size: 1.25rem;
  }
}
