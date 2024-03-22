# 👋 Hello, World! 
## I'm Rifat Al Jubayer 👨‍💻

<div align="center">
  <img src="https://media.giphy.com/media/LmNwrBhejkK9EFP504/giphy.gif" width="500" />
</div>

<p align="center">
  <samp>
    <b style="color: #FF6347;">🔭 Exploring:</b><br>
    Diving into various technology topics and satisfying my curiosity!
    <br><br>
    <b style="color: #20B2AA;">🌱 Learning:</b><br>
    Diving into advanced coding techniques and expanding my knowledge of programming languages.
    <br><br>
    <b style="color: #9370DB;">📫 How to reach me:</b><br>
    Drop me a message on <a href="https://twitter.com/Tayn511" style="color: #9370DB;">Twitter</a> or <a href="https://www.linkedin.com/in/rifat-al-jubayer" style="color: #9370DB;">LinkedIn</a>.
    <br><br>
    <b style="color: #2E8B57;">⚡ Fun fact:</b><br>
    I once hacked my own WiFi password just to see if I could!
  </samp>
</p>

<p align="center">
  <br><br>
  <b style="color: #9370DB;">📧 Contact:</b><br>
  Have questions or want to collaborate? Feel free to reach out via email at rifataljubaer2@gmail.com
</p>

<!-- Typewriter Effect Container -->
<p align="center" class="typewriter"></p>

<!-- Typewriter Effect Script -->
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
