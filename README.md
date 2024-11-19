# Project Responsive Web Design using Bootstrap
## Date:

## AIM:
To create a simplified clone of Dribbble (https://dribbble.com/) landing page.


## DESIGN STEPS:

### Step 1:
Clone the repository from GitHub.

### Step 2:
Create Django Admin project.

### Step 3:
Create a New App under the Django Admin project.

### Step 4:
Insert the necessary CSS and JavaScript files as external in order to use Bootstrap.

### Step 5:
Create a HTML file and include the needed Bootstrap components.

### Step 6:
Publish the website in the LocalHost.

## PROGRAM :
##html
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Dribbble Clone</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet">
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <!-- Navbar -->
  <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
    <div class="container">
      <a class="navbar-brand" href="#">Dribbble Clone</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav ms-auto">
          <li class="nav-item"><a class="nav-link active" href="#">Shots</a></li>
          <li class="nav-item"><a class="nav-link" href="#">Designers</a></li>
          <li class="nav-item"><a class="nav-link" href="#">Teams</a></li>
          <li class="nav-item"><a class="nav-link" href="#">Jobs</a></li>
        </ul>
      </div>
    </div>
  </nav>

  <!-- Hero Section -->
  <header class="bg-light text-center py-5">
    <div class="container">
      <h1 class="mb-3">Discover the world’s top designers</h1>
      <p class="lead">Dribbble is the go-to platform to showcase your design work.</p>
      <a href="#" class="btn btn-primary btn-lg me-2">Learn More</a>
      <a href="#" class="btn btn-outline-dark btn-lg">Sign Up</a>
    </div>
  </header>

  <!-- Gallery Section -->
  <main class="container py-5">
    <div class="row g-4">
      <!-- Card 1 -->
      <div class="col-md-4 col-sm-6">
        <div class="card">
          <img src="https://cdn.dribbble.com/userupload/16394212/file/original-c93733561f565d650dce4b759a417fb0.png?resize=400x300&vertical=center" class="card-img-top" alt="Sample Work 1">
          <div class="card-body">
            <p class="card-text">One week wonders</p>
          </div>
        </div>
      </div>
      <!-- Card 2 -->
      <div class="col-md-4 col-sm-6">
        <div class="card">
          <img src="https://cdn.dribbble.com/userupload/7588443/file/original-aefb88f1a1128b4511e0887ee07561b5.jpg?resize=400x300&vertical=center" class="card-img-top" alt="Sample Work 2">
          <div class="card-body">
            <p class="card-text">Television is a source of media</p>
          </div>
        </div>
      </div>
      <!-- Card 3 -->
      <div class="col-md-4 col-sm-6">
        <div class="card">
          <img src="https://cdn.dribbble.com/users/889819/screenshots/16809520/media/47ee015cba24d7d35cf35fc282612e93.png?resize=400x300&vertical=center" class="card-img-top" alt="Sample Work 3">
          <div class="card-body">
            <p class="card-text">A car's air conditioning (AC) system</p>
          </div>
        </div>
      </div>
      <!-- Card 4 -->
      <div class="col-md-4 col-sm-6">
        <div class="card">
          <img src="https://cdn.dribbble.com/userupload/10092239/file/original-96e3da362239ca0aa47a295b18e61dbe.png?resize=400x300&vertical=center" class="card-img-top" alt="Sample Work 4">
          <div class="card-body">
            <p class="card-text">A computer designed for personal use</p>
          </div>
        </div>
      </div>
      <!-- Card 5 -->
      <div class="col-md-4 col-sm-6">
        <div class="card">
          <img src="https://cdn.dribbble.com/userupload/7648770/file/still-31bf438b15ff4832ebcad1c58859f4b3.png?resize=400x300&vertical=center" class="card-img-top" alt="Sample Work 5">
          <div class="card-body">
            <p class="card-text">smart dashboard</p>
          </div>
        </div>
      </div>
      <div class="col-md-4 col-sm-6">
        <div class="card">
          <img src="https://cdn.dribbble.com/userupload/11438126/file/still-1cded3562249cd2125b72c65cacc0948.png?resize=400x300&vertical=center" class="card-img-top" alt="Sample Work 5">
          <div class="card-body">
            <p class="card-text">pocolo</p>
          </div>
        </div>
      </div>
    </div>
  </main>

  <!-- Footer -->
  <footer class="bg-dark text-center text-white py-3">
    <p class="mb-0">&copy; 2024 Dribbble Clone. All rights reserved.</p>
  </footer>

  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
```
##css
```
/* General Styles */
body {
    font-family: Arial, sans-serif;
  }
  
  header {
    background: linear-gradient(135deg, #f8f9fa, #e9ecef);
  }
  
  .navbar-brand {
    font-weight: bold;
  }
  
  .card {
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    transition: transform 0.2s, box-shadow 0.2s;
  }
  
  .card:hover {
    transform: scale(1.05);
    box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
  }
  
  footer {
    font-size: 0.9rem;
  }
```
##js
```
// JavaScript for Interactivity

// Sample data for filtering (optional)
const galleryItems = [
    { id: 1, category: "Popular", title: "Project by Famous" },
    { id: 2, category: "New", title: "Project by Balkan Brothers" },
    { id: 3, category: "Trending", title: "Project by Jan Losert" },
    { id: 4, category: "Popular", title: "Project by Mattias Johansson" },
    { id: 5, category: "Trending", title: "Project by Ruslan Siiz" }
  ];
  
  // Filter gallery items by category
  const filterButtons = document.querySelectorAll(".filter-btn");
  const gallery = document.querySelector(".row.g-4");
  
  filterButtons.forEach((btn) => {
    btn.addEventListener("click", () => {
      const category = btn.dataset.filter;
  
      // Clear existing gallery items
      gallery.innerHTML = "";
  
      // Add filtered items
      galleryItems
        .filter((item) => category === "All" || item.category === category)
        .forEach((item) => {
          gallery.innerHTML += `
            <div class="col-md-4 col-sm-6">
              <div class="card">
                <img src="https://via.placeholder.com/300" class="card-img-top" alt="${item.title}">
                <div class="card-body">
                  <p class="card-text">${item.title}</p>
                </div>
              </div>
            </div>
          `;
        });
    });
  });
  
  // Like button functionality
  document.addEventListener("click", (e) => {
    if (e.target.classList.contains("like-btn")) {
      const likesCount = e.target.querySelector(".likes-count");
      const count = parseInt(likesCount.textContent, 10);
      likesCount.textContent = count + 1;
    }
  });
```
## OUTPUT:

![project](https://github.com/user-attachments/assets/b469b8ab-4702-42c5-8804-b197a7d369d6)

## RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
