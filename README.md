<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HealthConnect Solar</title>
    <link rel="stylesheet" href="styles.css">
    <script src="script.js" defer></script>
</head>
<body>
    <header>
        <h1>Welcome to HealthConnect Solar</h1>
        <p>Empowering healthcare with sustainable solar solutions.</p>
        <nav>
            <ul>
                <li><a href="#about">About Us</a></li>
                <li><a href="#director">Our Director</a></li>
                <li><a href="#solutions">Our Solutions</a></li>
                <li><a href="#why-solar">Why Solar?</a></li>
                <li><a href="#data">Data Collection & Outreach</a></li>
                <li><a href="#government">Government Collaboration</a></li>
                <li><a href="#stories">Success Stories</a></li>
                <li><a href="#get-involved">Get Involved</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>
    
    <section id="donate">
        <h2>Support Our Mission</h2>
        <button onclick="donate()">Donate Now</button>
    </section>

    <section id="newsletter">
        <h2>Stay Updated</h2>
        <form id="newsletter-form">
            <input type="email" id="newsletter-email" placeholder="Enter your email" required>
            <button type="submit">Subscribe</button>
        </form>
        <p><a href="privacy-policy.html">Privacy Policy</a></p>
    </section>
    
    <section id="contact">
        <h2>Contact Us</h2>
        <form id="contact-form">
            <input type="text" id="contact-name" placeholder="Your Name" required>
            <input type="email" id="contact-email" placeholder="Your Email" required>
            <textarea id="contact-message" placeholder="Your Message" required></textarea>
            <button type="submit">Send Message</button>
        </form>
        <p>Email: <a href="mailto:healthconnectsolar@gmail.com">healthconnectsolar@gmail.com</a></p>
        <p>Phone: +233 2446 22 134</p>
    </section>
    
    <footer>
        <p>&copy; 2025 HealthConnect Solar. All Rights Reserved.</p>
        <p>Follow us on:
            <a href="https://www.facebook.com/healthconnectsolar" target="_blank">Facebook</a> |
            <a href="https://twitter.com/healthconnectsolar" target="_blank">Twitter</a> |
            <a href="https://www.instagram.com/healthconnectsolar" target="_blank">Instagram</a>
        </p>
    </footer>
    
    <script>
        document.addEventListener("DOMContentLoaded", function() {
            console.log("Script loaded successfully");
            
            document.getElementById("newsletter-form").addEventListener("submit", function(event) {
                event.preventDefault();
                let emailInput = document.getElementById("newsletter-email").value;
                let emailPattern = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
                
                console.log("Newsletter form submitted with email:", emailInput);
                
                if (!emailPattern.test(emailInput)) {
                    alert("Please enter a valid email address.");
                    console.log("Invalid email format");
                    return;
                }
                alert("Thank you for subscribing!");
                console.log("Subscription successful");
            });
            
            document.getElementById("contact-form").addEventListener("submit", function(event) {
                event.preventDefault();
                let nameInput = document.getElementById("contact-name").value;
                let emailInput = document.getElementById("contact-email").value;
                let messageInput = document.getElementById("contact-message").value;
                
                console.log("Contact form submitted with name:", nameInput, "email:", emailInput, "message:", messageInput);
                
                alert("Your message has been sent. We will get back to you soon.");
            });
        });
        
        function donate() {
            console.log("Donate button clicked");
            alert("Thank you for your support! You will be redirected to our donation page.");
            window.location.href = "donation_page.html";
        }
    </script>
</body>
</html>
# healthconnectsolar
