<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
<a name="readme-top"></a>
<!--
*** Thanks for checking out the Best-README-Template. If you have a suggestion
*** that would make this better, please fork the repo and create a pull request
*** or simply open an issue with the tag "enhancement".
*** Don't forget to give the project a star!
*** Thanks again! Now go create something AMAZING! :D
-->

<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->
[![Issues][issues-shield]][issues-url]

<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/patrickvorgers/SPC">
    <img src="images/SPC.png" alt="Logo" width="80" height="80">
  </a>

<h1 align="center">Smart Pump Control</h1>

  <p align="center">
    Are you tired of high electricity bills and inefficient heating systems in your home? The Smart Pump Control is the solution you've been waiting for. With this innovative device, you can enhance the performance of your heat pump in combination with central heating, ensuring optimal comfort, control and savings.
    <br />
    <br />
    <a href="https://github.com/patrickvorgers/SPC/issues">Report Bug</a>
    ·
    <a href="https://github.com/patrickvorgers/SPC/issues">Request Feature</a>
  </p>
</div>

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#installation">Installation</a></li>
        <li><a href="#restart_reset">Restart/Reset</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contact">Contact</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

<img src="images/SPC hardware.png">

### Floorheating usecase

Are you using floor heating and struggling with low temperature issues? The Smart Pump Control has the answer! By integrating this intelligent device into your heating system, you can optimize your energy consumption and maintain the perfect temperature in your home.

The Smart Pump Control is designed to work seamlessly with your heat pump and central heating system. It detects when either of these sources is producing heat and then intelligently activates your floor heating pump. This means you no longer have to keep the pump running continuously, wasting electricity when it's not needed. Instead, your heating system operates at its peak efficiency, saving you money on your energy bills.

### Take Control with Home Automation

With the Smart Pump Control, you're gaining more control. You can easily monitor and manage your Smart Pump Control through popular home automation systems like Home Assistant. Adjust settings from the convenience of your smartphone or computer. It's a smarter, more connected way to manage your pump.

### Key Benefits of Smart Pump Control:
<ul>
    <li>Energy Savings: Reduce electricity consumption by only running your pump when necessary.</li>
    <li>Home Automation Integration: Seamlessly integrate with Home Assistant or other automation systems for remote control.</li>
    <li>Easy Installation: Simple setup ensures you can start saving in no time.</li>
    <li>Temperature based activation but also on external state triggers.</li>
</ul>

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- GETTING STARTED -->
## Getting Started

Follow these simple steps to setup your Smart Pump Control

### Installation

1. Connect the temperature sensors to the device.
2. Plug the device in an electrical outlet
3. On your phone connect to the <b><i>SPC-S-AP</i></b> WiFi accesspoint for the socket version or to the <b><i>SPC-AP</i></b> WiFi accesspoint for the basic version and follow the steps to connect the Smart Pump Control to your WiFi network. It can take some time before the accessportal pops up so please be patient.
4. After the Smart Pump Control has been connected to the WiFi, the Smart Pump Control can be accessed via [http://spc-s.local](http://spc-s.local) for the socket version and on [http://spc.local](http://spc.local) for the basic version.
5. On the device page it is possible to rename the device into a more meaningfull name (needed when using multiple Smart Pump Control's on the same network)
6. Update the configuration to your liking

### Restart/Reset

#### Restart

Single press the button on the device. This will restart the device and preserve the configuration.

#### Configuration reset

Double press the button on the device. This will restart the device and reset all the settings to the factory defaults except for the WiFi connection.

#### Factory reset

Press and hold the button on the device for at least 3 seconds. This will restart the device and reset all the settings to the factory defaults including the WiFi connection.

<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- USAGE EXAMPLES -->
## Usage

### Web UI

<img src="images/SPC config.png">
<img src="images/SPC trigger.png">


### Home Assistant UI



<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- ROADMAP -->
## Roadmap

- [ ] Autodetect IP of the external trigger system based on the provided url
- [ ] Different pump activation temperatures for summer and winter
- [ ] Default behaviour when the external trigger system is not available (activate pump / deactivate pump)
- [ ] Delta triggering, when difference between two sensors is above a threshold activate the pump (scenario: difference between flow and return)

See the [open issues](https://github.com/patrickvorgers/SPC/issues) for a full list of proposed features (and known issues).

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- CONTACT -->
## Contact

Project Link: [https://github.com/patrickvorgers/SPC](https://github.com/patrickvorgers/SPC)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[issues-shield]: https://img.shields.io/github/issues/patrickvorgers/SPC.svg?style=for-the-badge
[issues-url]: https://github.com/patrickvorgers/SPC/issues
