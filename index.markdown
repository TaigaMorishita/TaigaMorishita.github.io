---
layout: page

carousels:
  - images: 
    - image: /assets/img/stm32_1.jpg
    - image: /assets/img/stm32_2.jpg
    - image: /assets/img/stm32_3.png
    - image: /assets/img/stm32_4.jpg

  - images: 
    - image: /assets/img/wsg1.jpg
    - image: /assets/img/wsg2.png
    - image: /assets/img/wsg3.jpg
    - image: /assets/img/staytuned.jpg

  - images: 
    - image: /assets/img/oven1.jpg
    - image: /assets/img/oven2.jpg
    - image: /assets/img/oven3.jpg
    - image: /assets/img/oven4.jpg

  - images: 
    - image: /assets/img/matilda1.png
    - image: /assets/img/matilda2.jpg
    - image: /assets/img/matilda3.png
    - image: /assets/img/matilda4.png

  - images: 
    - image: /assets/img/logintracker1.png
    - image: /assets/img/logintracker2.jpg
    - image: /assets/img/logintracker3.png
    - image: /assets/img/logintracker4.png

  - images: 
    - image: /assets/img/keyence1.png
    - image: /assets/img/keyence2.jpg
    - image: /assets/img/keyence3.png
    - image: /assets/img/keyence4.png
---

<style>
    /* Define Color Palette from _config.yml */
    :root {
        --purdue-black: {{ site.colors.purdue-black }};
        --purdue-gold: {{ site.colors.purdue-gold }};
        --purdue-gold-dark: {{ site.colors.purdue-gold-dark }};
        --light-bg: {{ site.colors.light-bg }};
        --text-color: {{ site.colors.text-color }};
        --carousel-bg: {{ site.colors.carousel-bg }};
        --white: {{ site.colors.white }};
    }

h2 {
    text-align: center;
    font-size: 1.5em;
    font-weight: bold;
}
    /* Global Reset and Typography */
    body {
        font-family: Arial, sans-serif;
        margin: 0;
        padding: 0;
        line-height: 1.6;
        color: var(--text-color);
        background-color: var(--light-bg);
        background-image: none;
        background-attachment: scroll;
    }

    .container {
        width: 90%;
        max-width: 1200px;
        margin: 0 auto;
        padding: 20px 0;
    }

    .hero {
        min-height: 450px;
        background-image: linear-gradient(rgba(255, 255, 255, 0.6), rgba(255, 255, 255, 0.6)), url('assets/img/banner.jpg');
        background-size: cover;
        background-position: center;
        background-repeat: no-repeat;
        position: relative;
    }

    .profile-pic {
        width: 300px;
        height: 300px;
        border-radius: 50%;
        object-fit: cover;
        border: 4px solid var(--purdue-gold);
        margin-bottom: 20px;
    }

    .hero-content h3 {
        color: var(--purdue-gold);
        font-weight: normal;
    }

    /* Buttons */
    .btn {
        display: inline-block;
        background-color: var(--purdue-gold);
        color: var(--purdue-black);
        padding: 10px 20px;
        margin-top: 20px;
        text-decoration: none;
        border-radius: 5px;
        font-weight: bold;
        transition: background-color 0.3s, transform 0.2s;
    }

    .btn:hover {
        background-color: var(--purdue-gold-dark);
        transform: translateY(-2px);
    }

    /* Skills Section */
    .skills-list ul {
        list-style: none;
        padding: 0;
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        gap: 20px;
        text-align: left;
    }

    .skills-list li {
        background-color: var(--white);
        border-left: 5px solid var(--purdue-gold);
        padding: 15px 20px;
        box-shadow: 0 2px 4px rgba(0, 0, 0, 0.05);
        flex: 1 1 45%;
        min-width: 300px;
    }

    /* Experience Section */
    .project-grid {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
        gap: 30px;
        margin-top: 30px;
        text-align: left;
    }

    .project-item {
        background-color: var(--white);
        padding: 20px;
        border-radius: 8px;
        box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        border-top: 5px solid var(--purdue-gold);
        transition: box-shadow 0.3s;
    }

    .project-item:hover {
        box-shadow: 0 6px 12px rgba(0, 0, 0, 0.15);
    }

    .project-item img {
        width: 100%;
        height: 200px;
        object-fit: cover;
        border-radius: 4px;
        margin-bottom: 15px;
    }

    .project-item a {
        display: inline-block;
        color: var(--purdue-gold);
        font-weight: bold;
        text-decoration: none;
        margin-top: 10px;
    }

  .project-row {
      display: flex;
      background-color: white;
      /* Keep content item white */
      border: 1px solid #ddd;
      border-radius: 8px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.05);
      margin-bottom: 40px;
      padding: 20px;
      text-align: left;
      align-items: center;
      gap: 30px;
  }

  .project-text {
      flex: 1;
      padding: 20px;
  }

  .project-text h3 {
      border-bottom: 2px solid var(--purdue-gold);
      padding-bottom: 5px;
      margin-bottom: 15px;
  }

          /* Skills Section (Kept white by default) */
        .skills-list ul {
            list-style: none;
            padding: 0;
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 20px;
            text-align: left;
        }

        .skills-list li {
            background-color: white;
            border-left: 5px solid var(--purdue-gold);
            padding: 15px 20px;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.05);
            flex: 1 1 45%;
            min-width: 300px;
        }

        .project-row {
            display: flex;
            background-color: white;
            /* Keep content item white */
            border: 1px solid #ddd;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.05);
            margin-bottom: 40px;
            padding: 20px;
            text-align: left;
            align-items: center;
            gap: 30px;
        }

        .project-text {
            flex: 1;
            padding: 20px;
        }

        hr {
    border: 0;
    height: 2px;
    background-color: var(--purdue-gold);
}
</style>

<section id="about" class="hero">
    <div class="container">
        <div class="hero-content">
            <img src="assets/img/headshot.jpg" alt="Headshot" class="profile-pic">
            <h2>Hi, I'm Taiga Morishita</h2>
            <h3>Engineering Technology Student | Purdue University</h3>
            <p>
                TODO
            </p>
            <a href="assets/Taiga Morishita Resume.pdf" class="btn" download>Download Resume (PDF)</a>
        </div>
    </div>
</section>

<hr>

<section id="skills" class="skills-section">
    <div class="container">
        <h2> Skills & Tools</h2>
        <div class="skills-list">
            <ul>
                <li><b>Design:</b> Onshape, SOLIDWORKS, Altium Designer, KiCad</li>
                <li><b>Certifications:</b> CISCO Certified Network Associate, AWS Cloud Pracitioner</li>
                <li><b>Data Analytics:</b> Python, MATLAB, Dash</li>
                <li><b>Programming:</b> PlatformIO, Bash, Embedded C++</li>
            </ul>
        </div>
    </div>
</section>

<hr>

<section id="experience" class="experience-section">
  <div class="container">
    <h2> Experience</h2>
    <div class="project-grid">

      <div class="project-item">
          <img src="assets/img/SIA-logo.png" alt="SIA Logo">
          <h3>Subaru of Indiana Automotive Internship</h3>
          <p>Interned at Subaru of Indiana Automotive as a Manufacturing Engineering intern from June 2025
              to August 2025.
              TODO</p>
      </div>

      <div class="project-item">
          <img src="assets/img/PBR.jpg" alt="Purdue Baja DAQ">
          <h3>Purdue Baja DAQ Member</h3>
          <p>Member of Purdue Baja Racing since September 2024. As part of the Baja SAE competition, we
              design, manufacture, test, and compete with a clean-sheet off-road vehicle every year.</p>
          <a href="https://www.purduebajaracing.com/" target="_blank">Learn More</a>
      </div>

      <div class="project-item">
          <img src="assets/img/nrg948.jpg" alt="NRG 948">
          <h3>NRG 948</h3>
          <p>TODO</p>
      </div>

    </div>
  </div>
</section>

<hr>

<section id="projects-detail" class="projects-detail-section">
  <div class="container">
    <h2> Detailed Projects</h2>

    <div class="project-row">
        <div class="project-text">
            <h3>Custom STM32 Sensor Board Development</h3>
            <p>Developed a custom STM32-based sensor TODO: finish</p>
        </div>
        <div style="flex: 1;">
            {% include carousel.html height="50" unit="%" duration="20" number="1" %}
        </div>
    </div>

    <div class="project-row">
        <div class="project-text">
            <h3>Wireless Strain Gage</h3>
            <p>WSG TODO</p>
        </div>
        <div style="flex: 1;">
            {% include carousel.html height="50" unit="%" duration="20" number="2" %}
        </div>
    </div>

    <div class="project-row">
        <div class="project-text">
            <h3>PCB Reflow Oven</h3>
            <p>Assisted in modifying a used toaster oven for PCB reflow to solder small SMD components for Purdue Baja Racing. Programmed an RP2040 using PlatformIO to read a Thermocouple and control a Solid State Relay, displaying information on a LCD screen.</p>
            <a href="https://github.com/PurdueBajaRacing/Reflow-Oven/tree/main" target="_blank">Code & Design Notes Here!</a>
        </div>
        <div style="flex: 1;">
            {% include carousel.html height="50" unit="%" duration="20" number="3" %}
        </div>
    </div>

    <!-- <div class="project-row">
        <div class="project-text">
            <h3>Tippy Cup</h3>
            <p>TODO/p>
        </div>
        <div style="flex: 1;">
            {% include carousel.html height="50" unit="%" duration="20" number="4" %}
        </div>
    </div> -->

    <!-- <div class="project-row">
        <div class="project-text">
            <h3>Attendance Tracking System</h3>
            <p>Programmed a Login/Logout app for FRC Team 948, connected to a Google Sheets. GUI made using Tkinter, with API connections to a complex Google Sheet with AppsScript to handle additional processing. Strong emphasis on easy of use and customizability.</p>
            <a href="hhttps://github.com/faletto/LoginTracker" target="_blank">See Code Here!</a>
        </div>
        <div style="flex: 1;">
            {% include carousel.html height="50" unit="%" duration="20" number="5" %}
        </div>
    </div> -->

    <!-- <div class="project-row">
        <div class="project-text">
            <h3>Keyence Laser Profiler Upgrade</h3>
            <p>LJ-X8000E</p>
        </div>
        <div style="flex: 1;">
            {% include carousel.html height="50" unit="%" duration="20" number="6" %}
        </div>
    </div> -->

  </div>
</section>
