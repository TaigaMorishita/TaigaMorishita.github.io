---
layout: page

carousels:
  - images: 
    - image: /assets/img/stm32_4.jpg
    - image: /assets/img/stm32_5.jpg
    - image: /assets/img/stm32_1.jpg
    - image: /assets/img/stm32_2.jpg
    - image: /assets/img/stm32_3.png

  - images: 
    - image: /assets/img/wsg1.jpg
    - image: /assets/img/wsg2.png
    - image: /assets/img/wsg3.jpg

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
    - image: /assets/img/logintracker2.png
    - image: /assets/img/logintracker3.png
    - image: /assets/img/logintracker4.png

  - images: 
    - image: /assets/img/keyence1.png
    - image: /assets/img/keyence2.jpg
    - image: /assets/img/keyence3.png
    - image: /assets/img/keyence4.png

  - images: 
    - image: /assets/img/jordanpranks1.png

  - images: 
    - image: /assets/img/pican1.png
    - image: /assets/img/pican2.jpg
    - image: /assets/img/pican3.png
    - image: /assets/img/pican4.png

  - images: 
    - image: /assets/img/nachi1.png
    - image: /assets/img/nachi2.jpg
    - image: /assets/img/nachi3.png
    - image: /assets/img/nachi4.png
---

<style>
    .site-header {
    position: sticky;
    top: 0;
    z-index: 1000;
    background-color: white;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}
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
            <h3><b>Engineering Technology Student | Purdue University</b></h3>
            <p>
                I am a Sophomore studying Automation and Systems Integration at Purdue University. My interests include aerospace, electronics (with a focus on microcontrollers), and technical theatre. I prioritize relentless optimization, efficiency, and process improvements, but even more importantly the ability to communicate and work in a team.
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
                <li><b>Data Analytics:</b> MATLAB, Dash, Pandas, Parquet</li>
                <li><b>Programming:</b> PlatformIO, Python, Ladder Logic, Structured Text, Bash, Embedded C++</li>
                <li><b>Certifications:</b> CISCO Certified Network Associate, AWS Certified Cloud Practitioner</li>
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
          <img src="assets/img/sia.jpg" alt="SIA Logo">
          <h3>Subaru of Indiana Automotive Intern - MfE Body</h3>
          <p>Interned at Subaru of Indiana Automotive as a Manufacturing Engineering intern - Body Section from June 2025
              to August 2025. 
              Implemented an upgrade to a Keyence Laser Profiler system, using a Mitsubishi Q-Series PLC to communicate between the measurement system and upstream data logging servers.
              Additionally reprogrammed over 100 Nachi robots to allow for certain checks to be bypassed during dry runs.</p>
      </div>

      <div class="project-item">
          <img src="assets/img/PBR.jpg" alt="Purdue Baja DAQ">
          <h3>Purdue Baja DAQ Member</h3>
          <p>Member of Purdue Baja Racing since September 2024. As part of the Baja SAE competition, we
              design, manufacture, test, and compete with a clean-sheet off-road vehicle every year. Data Acquisition (DAQ) designs and implements a wide variety of sensor data collection and analysis systems.</p>
          <a href="https://www.purduebajaracing.com/" target="_blank">Learn More</a>
      </div>

      <div class="project-item">
          <img src="assets/img/komo.jpg" alt="NRG 948">
          <h3>VP of Systems Engineering | Newport Robotics Group - FRC Team 948</h3>
          <p>In the <a href="https://www.firstinspires.org/programs/frc/" target="_blank">FIRST Robotics Competition (FRC)</a>, students design, build, program, test, and compete with a clean-sheet robot in just 8 weeks. Systems Engineering is a 20+ student subteam that creates a robust, impact-resistant electrical system carrying hundreds of amps of current.</p>
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
            <p>Developed a custom STM32F303K8U6-based sensor interface board, with UART, SWD, CAN, I2C, 8 MHz crystal, and analog support. Verified operation with an ESP32 as a CAN target, and created best practices for designing and programming custom PCB around bare ICs. Initial tests were done using a hand-soldered LQFP-32 STM32 on a breakout board, with a timing crystal and supporting circuitry added onto separate boards. These tests allowed for a fully functional sensor board on the first board revision.</p>
        </div>
        <div style="flex: 1;">
            {% include carousel.html height="50" unit="%" duration="20" number="1" %}
        </div>
    </div>

    <div class="project-row">
        <div class="project-text">
            <h3>Wireless Strain Gage</h3>
            <p>Designed and implemented a lightweight, fully wireless, torsional strain measurement system for Baja SAE vehicle axles. Worked closely with Drivetrain subsystem members to establish requirements and designed both the PCB and enclosure around axle dimensions.
            Used best practices form Omega and Vishay to design a performant strain gage processor in Altium, with high-precision, high-data-rate components and multiple auxiliary sensors. Data is send both wirelessly and saved to a local flash memory chip.
            </p>
        </div>
        <div style="flex: 1;">
            {% include carousel.html height="50" unit="%" duration="20" number="2" %}
        </div>
    </div>

    <!-- <div class="project-row">
        <div class="project-text">
            <h3>Tippy Cup</h3>
            <p>TODO
            <a href="https://example.com" target="_blank">See Design Notes Here!</a>
            </p>
        </div>
        <div style="flex: 1;">
            {% include carousel.html height="50" unit="%" duration="20" number="4" %}
        </div>
    </div> -->

    <div class="project-row">
        <div class="project-text">
            <h3>Attendance Tracking System</h3>
            <p>Created a Login/Logout system for FRC Team 948, connected to a Google Sheets. Programmed GUI made using Python and Tkinter, with API connections to a complex Google Sheet using AppsScript for additional processing. Strong emphasis placed on ease of use and customizability for team leaders. The system also privately sends emails to members upon request, allowing members to see their own attendance history.</p>
            <a href="https://github.com/faletto/LoginTracker" target="_blank">See Code Here!</a>
        </div>
        <div style="flex: 1;">
            {% include carousel.html height="50" unit="%" duration="20" number="5" %}
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
            <h3>Keyence Laser Profiler Upgrade</h3>
            <p>LJ-X8000E, GOT2000, Q-Series PLC. PLC-Link (an Ethernet-based protocol sometimes used in Japanese industrial controls)</p>
        </div>
        <div style="flex: 1;">
            {% include carousel.html height="50" unit="%" duration="20" number="6" %}
        </div>
    </div> -->

    <!-- <div class="project-row">
        <div class="project-text">
            <h3>Jordanian Pranks</h3>
            <p>TODO</p>
        </div>
        <div style="flex: 1;">
            {% include carousel.html height="50" unit="%" duration="20" number="7" %}
        </div>
    </div> -->

    <!-- <div class="project-row">
        <div class="project-text">
            <h3>Raspberry Pi CAN</h3>
            <p>TODO</p>
        </div>
        <div style="flex: 1;">
            {% include carousel.html height="50" unit="%" duration="20" number="8" %}
        </div>
    </div> -->

    <!-- <div class="project-row">
        <div class="project-text">
            <h3>Nachi Robot Reprogramming</h3>
            <p>TODO</p>
        </div>
        <div style="flex: 1;">
            {% include carousel.html height="50" unit="%" duration="20" number="9" %}
        </div>
    </div> -->

  </div>
</section>
