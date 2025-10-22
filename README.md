<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>SoulScope – Discover Your Inner Compass</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <h1>🧠 SoulScope</h1>
    <p>Discover your personality through playful quizzes</p>
    <nav>
      <a href="quiz.html">Take a Quiz</a>
    </nav>
  </header>
  <main>
    <section>
      <h2>Why SoulScope?</h2>
      <p>We believe self-awareness is the first step to happiness and prosperity. Our quizzes help you reflect, laugh, and grow.</p>
    </section>
  </main>
  body {
  font-family: 'Segoe UI', sans-serif;
  background: #f0f4f8;
  color: #333;
  margin: 0;
  padding: 0;
}
header {
  background: #4a90e2;
  color: white;
  padding: 20px;
  text-align: center;
}
nav a {
  color: white;
  margin: 0 10px;
  text-decoration: none;
}
main {
  padding: 20px;
}
footer {
  text-align: center;
  padding: 10px;
  background: #ddd;
}
  <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Take the Quiz</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <h1>🧠 Personality Quiz</h1>
  </header>
  <main>
    <form id="quizForm">
      <h3>1. How do you make decisions?</h3>
      <label><input type="radio" name="q1" value="logic"> Based on logic</label><br>
      <label><input type="radio" name="q1" value="emotion"> Based on emotions</label><br>

      <h3>2. What brings you joy?</h3>
      <label><input type="radio" name="q2" value="growth"> Learning and growth</label><br>
      <label><input type="radio" name="q2" value="connection"> Deep relationships</label><br>

      <button type="submit">See My Result</button>
    </form>
    <div id="result"></div>
  </main>
  <script src="quiz.js"></script>
</body>
</html>
  <footer>
    <p>Made with ❤️ by Ramandeep & Copilot</p>
    document.getElementById('quizForm').addEventListener('submit', function(e) {
  e.preventDefault();
  const q1 = document.querySelector('input[name="q1"]:checked');
  const q2 = document.querySelector('input[name="q2"]:checked');
  let result = '';

  if (q1 && q2) {
    if (q1.value === 'logic' && q2.value === 'growth') {
      result = "🧠 You're a Reflective Explorer!";
    } else if (q1.value === 'emotion' && q2.value === 'connection') {
      result = "💖 You're a Heartful Connector!";
    } else {
      result = "🌿 You're a Balanced Seeker!";
    }
    document.getElementById('result').innerText = result;
  } else {
    document.getElementById('result').innerText = "Please answer all questions.";
  }
});
  </footer>
</body>
</html>
