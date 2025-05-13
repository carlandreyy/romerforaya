<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Happy Anniversary, Aya!</title>
  <link href="https://fonts.googleapis.com/css2?family=Great+Vibes&family=Poppins:wght@300;600&display=swap" rel="stylesheet">
  <style>
    body {
      font-family: 'Poppins', sans-serif;
      margin: 0;
      padding: 0;
      background: linear-gradient(to right, #ffdde1, #ee9ca7);
      color: #333;
    }
    header {
      text-align: center;
      padding: 4rem 1rem;
      background: rgba(255, 255, 255, 0.6);
      backdrop-filter: blur(10px);
    }
    header h1 {
      font-family: 'Great Vibes', cursive;
      font-size: 3rem;
      color: #d6336c;
    }
    section {
      padding: 2rem;
      max-width: 800px;
      margin: auto;
      background: white;
      border-radius: 20px;
      box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
      margin-bottom: 2rem;
    }
    .gallery img {
      width: 100%;
      border-radius: 10px;
      margin: 1rem 0;
    }
    footer {
      text-align: center;
      font-size: 0.9rem;
      padding: 1rem;
    }
  </style>
</head>
<body>
  <audio autoplay loop>
    <source src="your-araw-araw-file.mp3" type="audio/mpeg">
  </audio>
  <header>
    <h1>Happy Anniversary, Aya 💖</h1>
    <p>From your one and only romerr — Andrei</p>
  </header>

  <section>
    <h2>Our Story</h2>
    <p>Before we met, love felt like a story na kulang ng ending. Parang may missing piece ako na hindi ko mahanap-hanap. Pero nung dumating ka, everything clicked. You filled the spaces I didn’t know were empty. Ikaw ang simula, gitna, at forever kong ending. 🥰</p>
  </section>

  <section>
    <h2>Gallery</h2>
    <div class="gallery">
      <!-- Upload your photos here -->
      <!-- Example: <img src="photos/photo1.jpg" alt="Us together"> -->
    </div>
  </section>

  <section>
    <h2>To My Aya 💌</h2>
    <p>Before we met, my understanding of love was like a puzzle missing a piece. I didn’t truly know what 'soulmate' meant until I found you, my romerr. Since the day you called me that, everything felt warmer, softer, more real. You’re the one who makes my world brighter, even on my worst days. Kahit tawagin mo akong Carl pag galit ka 😅, I’ll always be your Andrei — your romerr, your partner, your forever. 💗</p>
  </section>

  <section>
    <h2>Countdown to More Memories</h2>
    <p><strong>Anniversary:</strong> May 5, 2025</p>
    <div id="countdown"></div>
  </section>

  <footer>
    Made with 💖 by Romerr for Aya | Araw-Araw ng pagmamahal 🥰
  </footer>

  <script>
    const countdown = () => {
      const end = new Date('May 5, 2025 00:00:00').getTime();
      const now = new Date().getTime();
      const diff = end - now;
      if (diff < 0) {
        document.getElementById("countdown").innerHTML = "Happy Anniversary today, mahal! 🥳";
        return;
      }
      const days = Math.floor(diff / (1000 * 60 * 60 * 24));
      const hours = Math.floor((diff / (1000 * 60 * 60)) % 24);
      const mins = Math.floor((diff / (1000 * 60)) % 60);
      const secs = Math.floor((diff / 1000) % 60);
      document.getElementById("countdown").innerHTML = `${days} days ${hours} hrs ${mins} mins ${secs} secs left`;
    };
    setInterval(countdown, 1000);
  </script>
</body>
</html>
