<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="AI Learning Platform - Explore and Learn AI">
  <title>AI Learning Platform</title>
  <!-- External CSS link (Bootstrap for styling) -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">

  <style>
    body {
      background-color: #f4f6f9;
      font-family: Arial, sans-serif;
    }

    header {
      background-color: #0066cc;
      color: white;
      padding: 50px 0;
      text-align: center;
    }

    header h1 {
      font-size: 3rem;
    }

    .section-title {
      font-size: 2rem;
      margin-top: 40px;
      color: #333;
    }

    .card {
      margin-bottom: 20px;
    }

    .footer {
      background-color: #333;
      color: white;
      text-align: center;
      padding: 20px 0;
      position: absolute;
      width: 100%;
      bottom: 0;
    }

    .footer a {
      color: #00c4cc;
      text-decoration: none;
    }
  </style>
</head>

<body>

  <!-- Header Section -->
  <header>
    <h1>AI Learning Platform</h1>
    <p>Your journey to mastering AI starts here</p>
  </header>

  <!-- About Section -->
  <section class="container">
    <h2 class="section-title">About Us</h2>
    <p>Welcome to the AI Learning Platform! Whether you're a beginner or an expert, our goal is to provide high-quality
      resources and tutorials to help you learn Artificial Intelligence, Machine Learning, and Data Science. We offer
      interactive lessons, hands-on projects, and a community of learners.</p>
  </section>

  <!-- Course Offerings Section -->
  <section class="container">
    <h2 class="section-title">Our Courses</h2>
    <div class="row">
      <div class="col-md-4">
        <div class="card">
          <img src="https://via.placeholder.com/350x200" class="card-img-top" alt="Course 1">
          <div class="card-body">
            <h5 class="card-title">Intro to Machine Learning</h5>
            <p class="card-text">Learn the basics of Machine Learning, algorithms, and data analysis.</p>
            <a href="#" class="btn btn-primary">Start Learning</a>
          </div>
        </div>
      </div>
      <div class="col-md-4">
        <div class="card">
          <img src="https://via.placeholder.com/350x200" class="card-img-top" alt="Course 2">
          <div class="card-body">
            <h5 class="card-title">Deep Learning Essentials</h5>
            <p class="card-text">Dive into Neural Networks and Deep Learning techniques.</p>
            <a href="#" class="btn btn-primary">Start Learning</a>
          </div>
        </div>
      </div>
      <div class="col-md-4">
        <div class="card">
          <img src="https://via.placeholder.com/350x200" class="card-img-top" alt="Course 3">
          <div class="card-body">
            <h5 class="card-title">AI for Data Science</h5>
            <p class="card-text">Master the application of AI techniques in the world of Data Science.</p>
            <a href="#" class="btn btn-primary">Start Learning</a>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Resources Section -->
  <section class="container">
    <h2 class="section-title">Resources</h2>
    <ul>
      <li><a href="https://www.coursera.org" target="_blank">Coursera: AI & Machine Learning Courses</a></li>
      <li><a href="https://www.kaggle.com" target="_blank">Kaggle: Datasets & Competitions</a></li>
      <li><a href="https://www.fast.ai" target="_blank">Fast.ai: Deep Learning Courses</a></li>
      <li><a href="https://www.tensorflow.org" target="_blank">TensorFlow: Open Source ML Framework</a></li>
    </ul>
  </section>

  <!-- Contact Section -->
  <section class="container">
    <h2 class="section-title">Contact Us</h2>
    <p>If you have any questions or need help, feel free to contact us!</p>
    <form action="#" method="POST">
      <div class="mb-3">
        <label for="name" class="form-label">Your Name</label>
        <input type="text" class="form-control" id="name" name="name" required>
      </div>
      <div class="mb-3">
        <label for="email" class="form-label">Your Email</label>
        <input type="email" class="form-control" id="email" name="email" required>
      </div>
      <div class="mb-3">
        <label for="message" class="form-label">Your Message</label>
        <textarea class="form-control" id="message" name="message" rows="4" required></textarea>
      </div>
      <button type="submit" class="btn btn-primary">Submit</button>
    </form>
  </section>

  <!-- Footer Section -->
  <div class="footer">
    <p>&copy; 2024 AI Learning Platform. All Rights Reserved.</p>
    <p>Find us on <a href="https://github.com" target="_blank">GitHub</a> and <a href="https://twitter.com" target="_blank">Twitter</a>.</p>
  </div>

  <!-- External JS (Bootstrap JS) -->
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>

</body>

</html>
