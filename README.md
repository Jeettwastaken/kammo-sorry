<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>I'm Sorry Kammo 💖</title>
  <link href="https://fonts.googleapis.com/css2?family=Marcellus&family=Manrope:wght@400;600&display=swap" rel="stylesheet">
  <script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.12.2/gsap.min.js"></script>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    body {
      font-family: 'Manrope', sans-serif;
      background: linear-gradient(135deg, #ffe1ec, #f9dce3, #ffeef4);
      height: 100vh;
      overflow: hidden;
      display: flex;
      align-items: center;
      justify-content: center;
      flex-direction: column;
      color: #5c2c34;
    }

    .card {
      background: rgba(255, 255, 255, 0.4);
      border: 1px solid rgba(255, 182, 193, 0.4);
      box-shadow: 0 8px 32px rgba(255, 182, 193, 0.3);
      backdrop-filter: blur(10px);
      -webkit-backdrop-filter: blur(10px);
      border-radius: 18px;
      padding: 3em 2em;
      text-align: center;
      max-width: 700px;
      width: 90%;
      z-index: 2;
    }

    h1 {
      font-family: 'Marcellus', serif;
      font-size: 2.3rem;
      color: #c44569;
      margin-bottom: 1rem;
    }

    p {
      font-size: 1.1rem;
      line-height: 1.6;
      margin-bottom: 1.5rem;
      color: #6d3a4b;
    }

    .button-group {
      display: flex;
      justify-content: center;
      gap: 1rem;
      flex-wrap: wrap;
    }

    .button {
      background: #ff7e9e;
      border: none;
      color: #fff0f5;
      padding: 0.8rem 1.8rem;
      font-size: 1rem;
      font-weight: 600;
      border-radius: 30px;
      box-shadow: 0 0 12px rgba(255, 126, 158, 0.5);
      cursor: pointer;
      transition: all 0.3s ease;
    }

    .button:hover {
      background-color: #ffa6bc;
      transform: translateY(-2px);
    }

    .floating-heart {
      position: absolute;
      width: 20px;
      height: 20px;
      background: #ff9cb4;
      top: 100vh;
      left: 50%;
      transform: translateX(-50%) rotate(45deg);
      animation: float 10s linear infinite;
      opacity: 0.3;
    }

    .floating-heart::before,
    .floating-heart::after {
      content: "";
      position: absolute;
      width: 20px;
      height: 20px;
      background: #ff9cb4;
      border-radius: 50%;
    }

    .floating-heart::before {
      top: -10px;
      left: 0;
    }

    .floating-heart::after {
      top: 0;
      left: -10px;
    }

    @keyframes float {
      0% { top: 100vh; opacity: 0; }
      50% { opacity: 1; }
      100% { top: -20px; opacity: 0; }
    }

    audio {
      display: none;
    }
  </style>
</head>
<body>
  <div class="card">
    <h1>Sorry, Kammo 💖</h1>
    <p>Hey Dhreti, I know I crossed a line with that joke. It wasn’t funny, and I never meant to hurt you.</p>
    <p>
    Comedy is not my forte and mai thoda pagal bhi hoon, mujhe maafi chaiye
    </p>
    <p>You matter to me more than anyone else ever could, yeh seedney weedney koi nhi, tu hi hai bas meri jo hai</p>
    <div class="button-group">
      <button class="button" onclick="alert('aise ghatiya joke kabhi nhi marunga maaf kardo sweetu.')">chal maaf kiya</button>
      <button class="button" onclick="alert('You’re my person, always.')">sorry sundari</button>
    <button class="button" onclick="alert('I LOVE YOU BBGGGGGG.')">sorry itna delay karne ke liye, next time nhi hoga pakka </button>

    </div> 
    <audio autoplay loop>
      <source src="piya.mp3" type="audio/mpeg">
    </audio>
  </div>

  <script>
    for (let i = 0; i < 25; i++) {
      const heart = document.createElement('div');
      heart.classList.add('floating-heart');
      heart.style.left = Math.random() * 100 + 'vw';
      heart.style.animationDuration = (6 + Math.random() * 4) + 's';
      document.body.appendChild(heart);
    }

    gsap.from(".card", { scale: 0.8, opacity: 0, duration: 1.5, ease: "power3.out" });
  </script>
</body>
</html>
