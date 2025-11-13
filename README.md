hello
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <!-- <title>Beautiful HTML-Only Webpage</title> -->
</head>
<body>

  <!-- ===== Header Section ===== -->
  <header>
    <h1>🌸 Welcome to My Beautiful Web Page 🌸</h1>
    <p>Your one-stop destination for creative inspiration!</p>
    <hr>
  </header>

  <!-- ===== Navigation Links ===== -->
  <nav>
    <a href="#home">Home</a> |
    <a href="#about">About</a> |
    <a href="#gallery">Gallery</a> |
    <a href="#contact">Contact</a>
  </nav>

  <hr>

  <!-- ===== Home Section ===== -->
  <section id="home">
    <h2>🏠 Home</h2>
    <p>
      Welcome to this example of a large, well-structured webpage created using only HTML.  
      Although there’s no CSS or JavaScript, HTML alone allows us to organize content, insert images, and make it readable and structured.
    </p>
    <img src="https://th.bing.com/th/id/OIP.fwtcxV1lwwe8LBfvATENrQHaE7?w=278&h=185&c=7&r=0&o=7&cb=ucfimgc2&dpr=1.5&pid=1.7&rm=3" width="800" height="400">
    <p>
      The image above shows the beauty of nature — peaceful, colorful, and inspiring.  
      HTML is the skeleton of every webpage you see on the internet. It defines what each piece of content means.
    </p>
  </section>

  <hr>

  <!-- ===== About Section ===== -->
  <section id="about">
    <h2>💡 About Us</h2>
    <p>
      We are passionate creators who believe in simplicity and clarity.  
      This webpage is a demonstration of how far pure HTML can go in creating structure and meaning.  
      You can use HTML to build:
    </p>

    <ul>
      <li>Headings and paragraphs</li>
      <li>Links and navigation menus</li>
      <li>Images and multimedia elements</li>
      <li>Tables, forms, and lists</li>
    </ul>

    <p>
      Every great website starts with clean, semantic HTML — the foundation for design and functionality.
    </p>
  </section>

  <hr>

  <!-- ===== Gallery Section ===== -->
  <section id="gallery">
    <h2>🖼️ Image Gallery</h2>
    <p>Here are some beautiful images displayed using plain HTML:</p>

    <figure>
      <img src="https://th.bing.com/th/id/OIP.YKj7OrGcqWLugJN6YtlGawHaEK?w=331&h=180&c=7&r=0&o=7&cb=ucfimgc2&dpr=1.5&pid=1.7&rm=3" width="400" height="250">
      <figcaption>Sunset over mountains</figcaption>
    </figure>

    <figure>
      <img src="https://images.unsplash.com/photo-1500530855697-b586d89ba3ee" alt="Forest path" width="400" height="250">
      <figcaption>A peaceful forest path</figcaption>
    </figure>

    <figure>
      <img src="https://images.unsplash.com/photo-1482192596544-9eb780fc7f66" alt="City skyline" width="400" height="250">
      <figcaption>City skyline at night</figcaption>
    </figure>

    <p>
      Each image has a caption, and the layout is handled entirely by HTML’s <code>&lt;figure&gt;</code> and <code>&lt;figcaption&gt;</code> elements.
    </p>
  </section>

  <hr>

  <!-- ===== Table Section ===== -->
  <section>
    <h2>📊 Our Team</h2>
    <table border="1" cellpadding="10" cellspacing="0">
      <tr>
        <th>Name</th>
        <th>Role</th>
        <th>Location</th>
      </tr>
      <tr>
        <td>Alex Johnson</td>
        <td>Web Designer</td>
        <td>New York, USA</td>
      </tr>
      <tr>
        <td>Sophia Lee</td>
        <td>Photographer</td>
        <td>Seoul, South Korea</td>
      </tr>
      <tr>
        <td>Ravi Kumar</td>
        <td>Content Creator</td>
        <td>Delhi, India</td>
      </tr>
    </table>
  </section>

  <hr>

  <!-- ===== Contact Section ===== -->
  <section id="contact">
    <h2>📬 Contact Us</h2>
    <p>If you’d like to reach out, please fill out the simple form below:</p>

    <form>
      <label for="name">Your Name:</label><br>
      <input type="text" id="name" name="name"><br><br>

      <label for="email">Email Address:</label><br>
      <input type="email" id="email" name="email"><br><br>

      <label for="message">Your Message:</label><br>
      <textarea id="message" name="message" rows="5" cols="40"></textarea><br><br>

      <input type="submit" value="Send Message">
    </form>
  </section>

  <hr>

  <!-- ===== Footer ===== -->
  <footer>
    <p>&copy; 2025 My Beautiful HTML Page | Designed with ❤️ using only HTML</p>
  </footer>

</body>
</html>
