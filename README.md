# CharityWater
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Charity Water Landing Page</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <link rel="stylesheet" href="style.css" />
</head>
<body class="bg-yellow-400 relative overflow-hidden">

  <!-- Animated Droplets -->
  <script>
    document.addEventListener('DOMContentLoaded', () => {
      for (let i = 0; i < 20; i++) {
        const drop = document.createElement('div');
        drop.classList.add('droplet');
        drop.style.left = `${Math.random() * 100}vw`;
        drop.style.animationDuration = `${3 + Math.random() * 2}s`;
        drop.style.animationDelay = `${Math.random() * 5}s`;
        document.body.appendChild(drop);
      }
    });
  </script>

  <div class="flex min-h-screen items-center justify-center bg-yellow-400">
    <div class="flex flex-col md:flex-row w-full max-w-screen-xl bg-white overflow-hidden shadow-lg">

      <!-- Left Image Section -->
      <div class="md:w-1/2 w-full h-[70vh] md:h-auto relative">
        <img
          src="your-image-path.jpg"
          alt="Child with clean water"
          class="object-cover w-full h-full"
        />
      </div>

      <!-- Right Content Section -->
      <div class="md:w-1/2 w-full bg-white p-8 flex flex-col justify-center">
        <!-- Logo -->
        <div class="mb-4">
          <img src="logo-placeholder.png" alt="charity: water logo" class="w-48"/>
        </div>

        <!-- Headline -->
        <h1 class="text-3xl font-semibold mb-2 text-gray-800">
          Small Drops Together<br />
          <span class="text-black font-bold">Become a Life-Giving Stream</span>
        </h1>

        <!-- Paragraph -->
        <p class="text-gray-600 mt-4 mb-4 text-sm leading-relaxed">
          When you give, you do more than provide water—you give time back to families, open doors to education, protect health, and spark opportunity for generations.<br/>
          <strong>It starts with you.</strong>
        </p>

        <!-- CTA -->
        <p class="text-blue-600 font-medium mt-4">
          💧 Be the drop. Give clean water.
        </p>
      </div>

    </div>
  </div>

</body>
</html>
@keyframes dropletFall {
  0% {
    transform: translateY(-100%);
    opacity: 0;
  }
  50% {
    opacity: 1;
  }
  100% {
    transform: translateY(100vh);
    opacity: 0;
  }
}

.droplet {
  position: absolute;
  width: 8px;
  height: 8px;
  background-color: rgba(59, 130, 246, 0.8);
  border-radius: 50%;
  animation: dropletFall linear infinite;
}  
