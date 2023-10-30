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
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
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

Are you using floor heating and struggling with low temperature issues? The Smart Pump Control has the answer! By integrating this intelligent device into your heating system, you can optimize your energy consumption and maintain the perfect temperature in your home.

### Efficiency at Its Best

The Smart Pump Control is designed to work seamlessly with your heat pump and central heating system. It detects when either of these sources is producing heat and then intelligently activates your floor heating pump. This means you no longer have to keep the pump running continuously, wasting electricity when it's not needed. Instead, your heating system operates at its peak efficiency, saving you money on your energy bills.

### Take Control with Home Automation

With the Smart Pump Control, you're not only improving your heating system's efficiency but also gaining more control. You can easily monitor and manage your Smart Pump Control through popular home automation systems like Home Assistant. Adjust settings, track energy consumption, and set schedules from the convenience of your smartphone or computer. It's a smarter, more connected way to manage your home's heating system.

### Key Benefits of Smart Pump Control:
<ol>
    <li>Energy Savings: Reduce electricity consumption by only running your floor heating pump when necessary.</li>
    <li>Improved Comfort: Maintain consistent and comfortable temperatures throughout your home.</li>
    <li>Home Automation Integration: Seamlessly integrate with Home Assistant or other automation systems for remote control.</li>
    <li>Easy Installation: Simple setup ensures you can start saving and optimizing your heating system in no time.</li>
</ol>

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- GETTING STARTED -->
## Getting Started

This is an example of how you may give instructions on setting up your project locally.
To get a local copy up and running follow these simple example steps.

### Prerequisites

This is an example of how to list things you need to use the software and how to install them.
* npm
  ```sh
  npm install npm@latest -g
  ```

### Installation

1. Get a free API Key at [https://example.com](https://example.com)
2. Clone the repo
   ```sh
   git clone https://github.com/patrickvorgers/SPC.git
   ```
3. Install NPM packages
   ```sh
   npm install
   ```
4. Enter your API in `config.js`
   ```js
   const API_KEY = 'ENTER YOUR API';
   ```

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- USAGE EXAMPLES -->
## Usage

Use this space to show useful examples of how a project can be used. Additional screenshots, code examples and demos work well in this space. You may also link to more resources.

_For more examples, please refer to the [Documentation](https://example.com)_

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
