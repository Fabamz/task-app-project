<template>
  <div class="about-container">
    <div class="header">
      <h2>About Task Tracker</h2>
      <router-link to="/" class="home-link">TrackApp Home Page</router-link>
    </div>

    <section class="features">
      <h3>Features</h3>
      <ul>
        <li>Track and manage your tasks with ease</li>
        <li>Set reminders for important deadlines</li>
      </ul>
    </section>

    <section class="about-dev">
      <h3>About the Developer</h3>
      <p>
        TaskTracker was developed by <strong>Adeyemi Bamidele</strong>, a
        passionate software developer dedicated to creating simple and effective
        solutions for productivity.
      </p>
      <p>Feel free to connect and get updates on this project via:</p>
      <ul>
        <li><a href="https://github.com/Fabamz" target="_blank">GitHub</a></li>
        <li>
          <a href="https://www.linkedin.com/in/adeyemibamidele" target="_blank"
            >LinkedIn</a
          >
        </li>
      </ul>
    </section>

    <section class="contact">
      <h3>Contact Us</h3>
      <p>If you have any questions or feedback, feel free to reach out:</p>
      <ul>
        <li>
          Email:
          <a href="mailto:adeyemibamidele03@yahoo.com">info@fabamz.com</a>
        </li>
        <li>Phone: +1 (860) 328-1137</li>
      </ul>
    </section>
  </div>
</template>

<style scoped>
.about-container {
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  align-items: center;
  font-family: "Arial", sans-serif;
  padding: 20px;
  max-width: 1200px;
  margin: 0 auto;
  background-color: #f4f7fa;
  border-radius: 10px;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
  color: #333;
}

.header {
  text-align: center;
  margin-bottom: 30px;
  padding: 20px;
  box-shadow: 0 4px 12px rgba(0, 0, 255, 0.2);
  background-color: rgb(245, 245, 245);
  width: 100%;
}

.header h2 {
  font-size: 1.5em;
  color: #2c3e50;
  margin-bottom: 10px;
}

.home-link {
  display: inline-block;
  margin-top: 20px;
  font-size: 1.1em;
  color: rgb(41, 128, 185);
  text-decoration: none;
  border: 2px solid rgb(41, 128, 185);
  padding: 8px 16px;
  border-radius: 30px;
  transition: all 0.3s ease-in-out;
}

.home-link:hover {
  color: white;
  background-color: rgb(41, 128, 185);
  transform: scale(1.1);
}

.features {
  margin-bottom: 40px;
  padding: 20px;
  box-shadow: 0 4px 12px rgba(0, 255, 0, 0.2);
  background-color: rgb(255, 255, 255);
  width: 100%;
}

.features h3 {
  font-size: 1.2em;
  color: rgb(44, 62, 80);
  margin-bottom: 15px;
}

.features ul {
  list-style: none;
  padding: 0;
  font-size: 1.1em;
  color: rgb(52, 73, 94);
}

.features li {
  margin-bottom: 10px;
}

.about-dev {
  margin-bottom: 40px;
  padding: 20px;
  box-shadow: 0 4px 12px rgba(255, 0, 0, 0.2);
  background-color: #fff;
  width: 100%;
}

.about-dev h3 {
  font-size: 1.2em;
  color: rgb(44, 62, 80);
  margin-bottom: 15px;
}

.about-dev p {
  font-size: 1.1em;
  color: rgb(52, 73, 94);
  margin-bottom: 15px;
}

.about-dev ul {
  list-style: none;
  padding: 0;
}

.about-dev li {
  margin-bottom: 10px;
}

.about-dev a {
  color: rgb(41, 128, 185);
  text-decoration: none;
}

.about-dev a:hover {
  text-decoration: underline;
  color: rgb(0, 0, 255);
}

.contact {
  margin-bottom: 40px;
  padding: 20px;
  box-shadow: 0 4px 12px rgba(255, 165, 0, 0.2);
  background-color: rgb(255, 255, 255);
  width: 100%;
}

.contact h3 {
  font-size: 1.2em;
  color: rgb(44, 62, 80);
  margin-bottom: 15px;
}

.contact ul {
  list-style: none;
  padding: 10px;
  font-size: 1.1em;
  color: rgb(52, 73, 94);
}

.contact li {
  margin-bottom: 10px;
}
</style>
