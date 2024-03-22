<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Rifat Al Jubayer's GitHub Profile</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #f8f9fa;
      color: #495057;
    }
    .container {
      max-width: 800px;
      margin: 0 auto;
      padding: 20px;
    }
    .header img {
      width: 100%;
      border-radius: 10px;
    }
    .profile-info {
      text-align: center;
    }
    .profile-info h2 {
      margin-bottom: 10px;
    }
    .profile-info p {
      margin-bottom: 20px;
    }
    .contact-info {
      margin-top: 50px;
      text-align: center;
    }
    .contact-info a {
      margin: 0 10px;
      color: #9370DB;
      text-decoration: none;
    }
    .contact-info a:hover {
      text-decoration: underline;
    }
    .typewriter {
      font-size: 18px;
      font-weight: bold;
    }
  </style>
</head>
<body>
  <div class="container">
    <div class="header">
      <h1 align="center">👋 Hello, World!</h1>
      <h2 align="center">I'm Rifat Al Jubayer 👨‍💻</h2>
      <div align="center">
        <img src="https://media.giphy.com/media/LmNwrBhejkK9EFP504/giphy.gif" alt="Welcome Gif">
      </div>
    </div>
    <div class="profile-info">
      <h3>🔭 Exploring:</h3>
      <p>Diving into various technology topics and satisfying my curiosity!</p>
      <h3>🌱 Learning:</h3>
      <p>Diving into advanced coding techniques and expanding my knowledge of programming languages.</p>
    </div>
    <div class="contact-info">
      <h3>📫 How to reach me:</h3>
      <p>Drop me a message on <a href="https://twitter.com/Tayn511">Twitter</a> or <a href="https://www.linkedin.com/in/rifat-al-jubayer">LinkedIn</a>.</p>
      <h3>📧 Contact:</h3>
      <p>Have questions or want to collaborate? Feel free to reach out via email at rifataljubaer2@gmail.com.</p>
    </div>
    <div class="typewriter" align="center"></div>
  </div>

  <script>
    const txtElement = document.querySelector('.typewriter');
    const words = ["Welcome to My GitHub Profile!", "I'm Rifat Al Jubayer, a passionate self-taught Hacker", "I Love Solving Cyber Puzzles"];
    let wordIndex = 0;
    let charIndex = 0;

    function type() {
      if (charIndex < words[wordIndex].length) {
        txtElement.textContent += words[wordIndex].charAt(charIndex);
        charIndex++;
        setTimeout(type, 100);
      } else {
        setTimeout(erase, 1500);
      }
    }

    function erase() {
      if (charIndex > 0) {
        txtElement.textContent = words[wordIndex].substring(0, charIndex - 1);
        charIndex--;
        setTimeout(erase, 50);
      } else {
        wordIndex++;
        if (wordIndex >= words.length) wordIndex = 0;
        setTimeout(type, 500);
      }
    }

    type();
  </script>
</body>
</html>
