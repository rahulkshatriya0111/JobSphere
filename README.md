(http://localhost:3000/index.html)                                                                           # JobSphere

#index.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>JobSphere - Find Your Dream Job</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <nav>
            <ul>
                <li><a href="index.html">Home</a></li>
                <li><a href="about.html">About</a></li>
                <li><a href="contact.html">Contact</a></li>
                <li><a href="login.html">Login</a></li>
                <li><a href="register.html">Register</a></li>
            </ul>
        </nav>
    </header>

    <section class="hero">
        <div class="hero-content">
            <h1>Welcome to JobSphere</h1>
            <p>Your next job is just a click away</p>
            <form class="search-form">
                <input type="text" placeholder="Search for jobs..." id="search-input">
                <button type="submit">Search</button>
            </form>
        </div>
    </section>

    <section class="featured-jobs">
        <h2>Featured Jobs</h2>
        <div class="job-listings">
            <!-- Sample job listing -->
            <div class="job-card">
                <h3>Software Engineer</h3>
                <p>Company Name</p>
                <a href="job-detail.html">View Details</a>
            </div>
            <div class="job-card">
                <h3>Web Developer</h3>
                <p>Company Name</p>
                <a href="job-detail.html">View Details</a>
            </div>
        </div>
    </section>

    <footer>
        <p>&copy; 2025 JobSphere. All rights reserved.</p>
    </footer>

    <script src="assets/js/script.js"></script>
</body>
</html>

#about.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>About JobSphere</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <nav>
            <ul>
                <li><a href="index.html">Home</a></li>
                <li><a href="about.html">About</a></li>
                <li><a href="contact.html">Contact</a></li>
                <li><a href="login.html">Login</a></li>
                <li><a href="register.html">Register</a></li>
            </ul>
        </nav>
    </header>

    <section class="about">
        <div class="about-header">
            <h1>Welcome to JobSphere</h1>
            <p>Your career journey starts here</p>
        </div>

        <div class="about-content">
            <div class="about-text">
                <h2>Who We Are</h2>
                <p>JobSphere is a modern job portal that connects employers with job seekers. Our mission is to help people find meaningful work and assist companies in hiring the best talent. Whether you're looking for your first job, a career change, or a high-level executive role, JobSphere is here to help you at every step.</p>
                
                <h2>Our Vision</h2>
                <p>We aim to revolutionize the job search process by providing a seamless, intuitive platform where individuals can explore job opportunities, apply to positions, and grow their careers. Our platform is designed to connect employers with highly skilled professionals across various industries.</p>

                <h2>How JobSphere Works</h2>
                <p>JobSphere offers a user-friendly interface for both job seekers and employers. Job seekers can create profiles, upload resumes, and search for job listings that match their skills and experience. Employers can post job openings, filter candidates, and hire directly from the platform. With JobSphere, job searching and hiring has never been easier.</p>
            </div>

            <div class="about-images">
                <div class="image-container">
                    <img src="https://th.bing.com/th/id/OIP.n3dcxPYqkDTauNaJnXLKTwHaDr?rs=1&pid=ImgDetMain" alt="Job Search" />
                    <p>Explore Job Opportunities</p>
                </div>
                <div class="image-container">
                    <img src="https://th.bing.com/th/id/OIP.UXVg_yF-YeGz7phNloivIwAAAA?w=247&h=180&c=7&r=0&o=5&pid=1.7" alt="Job Applications" />
                    <p>Submit Your Application</p>
                </div>
            </div>
        </div>

        <!-- Next Button Section -->
        <div class="next-button-container ">
            <a href="contact.html" class="next-button">Next &rarr;</a>
        </div>
    </section>

    <footer>
        <p>&copy; 2025 JobSphere. All rights reserved.</p>
    </footer>

    <script src="assets/js/script.js"></script>
</body>
</html>

#contact.html
#login.html
#register.html

#script.js

// Simple search functionality (for now, just logs the search term)
document.querySelector('.search-form').addEventListener('submit', function (event) {
    event.preventDefault();
    const searchQuery = document.getElementById('search-input').value;
    console.log("Searching for: " + searchQuery);
});


#styles.css
/* Reset some basic styles */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    background-color: #f4f4f4;
    color: #333;
}

/* Header Navigation */
header {
    background-color: #2e775b;
    padding: 10px 0;
}

header nav ul {
    display: flex;
    justify-content: center;
    list-style-type: none;
}

header nav ul li {
    margin: 0 20px;
}

header nav ul li a {
    color: white;
    text-decoration: none;
    font-size: 18px;
}

/* Hero Section */
.hero {
    background-color: #2e775b;
    color: white;
    text-align: center;
    padding: 100px 0;
}

.hero h1 {
    font-size: 3rem;
    margin-bottom: 20px;
}

.hero .search-form {
    margin-top: 20px;
}

.hero input {
    width: 300px;
    padding: 10px;
    border-radius: 25px;
    border: none;
    font-size: 16px;
}

.hero button {
    padding: 10px 20px;
    margin-left: 10px;
    border-radius: 25px;
    background-color: #f4a261;
    border: none;
    cursor: pointer;
}

.hero button:hover {
    background-color: #e76f51;
}

/* Featured Jobs Section */
.featured-jobs {
    padding: 50px 20px;
    text-align: center;
}

.job-listings {
    display: flex;
    justify-content: center;
    gap: 20px;
}

.job-card {
    background-color: white;
    padding: 20px;
    border-radius: 10px;
    box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.1);
    width: 250px;
}

.job-card h3 {
    font-size: 1.5rem;
    color: #2e775b;
}

.job-card p {
    color: #777;
    margin: 10px 0;
}

.job-card a {
    text-decoration: none;
    color: #2e775b;
    font-weight: bold;
}

.job-card a:hover {
    color: #f4a261;
}

/* Footer */
footer {
    text-align: center;
    background-color: #2e775b;
    color: white;
    padding: 20px 0;
}
/* About Page Styling */
.about {
    padding: 50px 20px;
    text-align: center;
}

.about-header {
    margin-bottom: 40px;
}

.about-header h1 {
    font-size: 2.5rem;
    color: #2e775b;
}

.about-header p {
    font-size: 1.2rem;
    color: #555;
}

.about-content {
    display: flex;
    justify-content: space-between;
    gap: 40px;
    flex-wrap: wrap;
    margin-top: 40px;
}

.about-text {
    flex: 1;
    max-width: 600px;
    text-align: left;
}

.about-text h2 {
    font-size: 2rem;
    margin-bottom: 10px;
    color: #2e775b;
}

.about-text p {
    margin-bottom: 20px;
    line-height: 1.6;
    color: #777;
}

.about-images {
    flex: 1;
    display: flex;
    gap: 20px;
    justify-content: center;
    flex-wrap: wrap;
}

.image-container {
    text-align: center;
}

.image-container img {
    width: 100%;
    max-width: 400px;
    height: auto;
    border-radius: 8px;
    margin-bottom: 10px;
}

.image-container p {
    color: #2e775b;
    font-weight: bold;
}


/* Next Button Styling */
.next-button-container {
    margin-top: 40px;
    text-align: center;
}

.next-button {
    background-color: #2e775b;
    color: white;
    padding: 15px 30px;
    font-size: 1.2rem;
    text-decoration: none;
    border-radius: 25px;
    transition: background-color 0.3s ease;
}

.next-button:hover {
    background-color: #f4a261;
}
