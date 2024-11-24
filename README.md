<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Mert's Blog</title>
  <style>
    /* General styles */
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background-color: #f4f4f4;
    }

    header {
      background-color: #333;
      color: white;
      padding: 20px;
      text-align: center;
    }

    nav ul {
      list-style: none;
      padding: 0;
    }

    nav ul li {
      display: inline;
      margin: 0 10px;
    }

    nav ul li a {
      color: white;
      text-decoration: none;
    }

    section {
      margin: 20px;
    }

    footer {
      text-align: center;
      background-color: #333;
      color: white;
      padding: 10px;
    }

    .intro, .featured-posts, .about, .blog-posts, .post-detail, .contact {
      margin-bottom: 40px;
    }

    #comment-section {
      margin-top: 20px;
    }

    #comment-input {
      width: 100%;
      height: 100px;
    }

    button {
      margin-top: 10px;
      padding: 10px 20px;
      background-color: #333;
      color: white;
      border: none;
      cursor: pointer;
    }

    form input, form textarea {
      width: 100%;
      padding: 10px;
      margin-bottom: 10px;
    }

    form button {
      padding: 10px 20px;
      background-color: #333;
      color: white;
      border: none;
      cursor: pointer;
    }
  </style>
</head>
<body>

  <!-- Header -->
  <header>
    <h1>Mert's Blog</h1>
    <nav>
      <ul>
        <li><a href="#home">Home</a></li>
        <li><a href="#blog">Blog Posts</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  <!-- Home Page -->
  <section id="home" class="intro">
    <h2>Welcome to My Blog!!!</h2>
    <p>This blog is all about discovering new countries to visit, exploring the best places, cultures, and travel tips!</p>
  </section>

  <!-- Blog Posts -->
  <section id="blog" class="blog-posts">
    <h2>Featured Posts</h2>
    <ul>
      <li><a href="#post1">Top Countries to Visit in Europe</a></li>
      <li><a href="#post2">Best Travel Destinations for 2024</a></li>
      <li><a href="#post3">A Complete Guide to Backpacking</a></li>
    </ul>
  </section>

  <!-- Post Details -->
  <section id="post1" class="post-detail">
    <h2>Top Countries to Visit in Europe</h2>
    <p>Author: Mert Özer | Date: November 24, 2024</p>
    <p>Europe is a continent filled with diverse cultures and landscapes. Here are the top countries you should visit in Europe...</p>

    <h3>Comments</h3>
    <div id="comment-section">
      <textarea id="comment-input" placeholder="Leave a comment..."></textarea>
      <button onclick="postComment()">Submit Comment</button>
      <div id="comments"></div>
    </div>
  </section>

  <!-- About Section -->
  <section id="about" class="about">
    <h2>About Me</h2>
    <p>My name is Mert Özer, and I am 21 years old. I am currently studying at Okan University, where I am pursuing my academic journey. My passion lies in exploring new places, cultures, and countries, which is the primary theme of this blog.</p>
  </section>

  <!-- Contact Section -->
  <section id="contact" class="contact">
    <h2>Contact Me</h2>
    <form action="#">
      <label for="name">Your Name</label>
      <input type="text" id="name" name="name" required>

      <label for="email">Your Email</label>
      <input type="email" id="email" name="email" required>

      <label for="message">Your Message</label>
      <textarea id="message" name="message" required></textarea>

      <button type="submit">Send Message</button>
    </form>

    <p>Feel free to reach out to me via email at <a href="mailto:mertozer2003@hotmail.com">mertozer2003@hotmail.com</a>.</p>
    <p>Or follow me on Instagram: <a href="https://www.instagram.com/mertozer.zg" target="_blank">Instagram Profile</a></p>
  </section>

  <!-- Footer -->
  <footer>
    <p>&copy; 2024 Mert's Blog</p>
  </footer>

  <script>
    // Function to post comment
    function postComment() {
      const commentInput = document.getElementById('comment-input');
      const commentSection = document.getElementById('comments');
      const comment = document.createElement('p');
      comment.textContent = commentInput.value;
      commentSection.appendChild(comment);
      commentInput.value = ''; // Clear input after comment is posted
    }
  </script>

</body>
</html>
