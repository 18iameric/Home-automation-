# Home-automation-
Install services 
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Home Automation Services</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <header>
    <h1>Smart Home Solutions</h1>
    <p>Your trusted partner for Home Automation Installation and Maintenance</p>
  </header>
  
  <nav>
    <ul>
      <li><a href="#services">Services</a></li>
      <li><a href="#highlights">Highlights</a></li>
      <li><a href="#contact">Contact Us</a></li>
    </ul>
  </nav>

  <section id="services">
    <h2>Our Services</h2>

    <div class="service-card">
      <h3>Basic Home Automation Integration</h3>
      <p>Onboard your existing home automation devices to the Home Assistant platform, ensuring seamless compatibility with all smartphones.</p>
      <p><strong>Package Price: $499</strong></p>
    </div>

    <div class="service-card">
      <h3>All-Inclusive Lighting Package</h3>
      <p>Integrate all your home's lighting into the Home Assistant platform. This package includes up to 6 lights. Additional lights cost $50 per light.</p>
      <p><strong>Package Price: $899</strong></p>
    </div>
  </section>

  <section id="highlights">
    <h2>What Home Assistant Can Do for You</h2>
    <ul>
      <li>Control all your devices from a single app on your smartphone or tablet.</li>
      <li>Set up custom automations, such as lights turning on at sunset or your thermostat adjusting when you leave home.</li>
      <li>Monitor your home with real-time alerts and notifications.</li>
      <li>Ensure compatibility with a wide range of smart devices, from lights to security cameras.</li>
      <li>Enable voice control through Amazon Alexa, Google Assistant, or Apple Siri.</li>
      <li>Enhance energy efficiency with detailed usage statistics and automations.</li>
    </ul>
  </section>

  <footer id="contact">
    <h2>Contact Us</h2>
    <p>Ready to transform your home? Get in touch!</p>
    <p>Email: info@smarthomesolutions.com</p>
    <p>Phone: (123) 456-7890</p>
  </footer>
  
  <script src="script.js"></script>
</body>
</html>

body {
  font-family: Arial, sans-serif;
  line-height: 1.6;
  margin: 0;
  padding: 0;
}

header {
  background: #00796b;
  color: white;
  padding: 20px;
  text-align: center;
}

nav ul {
  background: #004d40;
  color: white;
  display: flex;
  justify-content: center;
  list-style: none;
  margin: 0;
  padding: 10px 0;
}

nav ul li {
  margin: 0 15px;
}

nav ul li a {
  color: white;
  text-decoration: none;
}

section {
  margin: 20px;
  padding: 20px;
}

h2 {
  border-bottom: 2px solid #00796b;
  padding-bottom: 5px;
}

.service-card {
  background: #e0f2f1;
  border: 1px solid #00796b;
  border-radius: 5px;
  margin: 15px 0;
  padding: 15px;
}

footer {
  background: #004d40;
  color: white;
  padding: 20px;
  text-align: center;
}

footer p {
  margin: 5px 0;
}

// Add dynamic pricing for additional lights
const additionalLightCost = 50;
const baseLightCount = 6;

function calculateTotalLights(basePrice, additionalLights) {
  const extraCost = additionalLights > baseLightCount ? 
    (additionalLights - baseLightCount) * additionalLightCost : 0;
  return basePrice + extraCost;
}

console.log("Total price for 10 lights: $" + calculateTotalLights(899, 10));
