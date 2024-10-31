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
    <img src="https://raw.githubusercontent.com/patrickvorgers/SPC/main/images/SPC.png" alt="Logo" width="80" height="80">
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
        <li><a href="#restart-reset">Restart/Reset</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
      <ul>
        <li><a href="#temperature-activation">Temperature activation</a></li>
        <li><a href="#web-ui">Web UI</a></li>
        <li><a href="#home-assistant-ui">Home Assistant UI</a></li>
      </ul>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contact">Contact</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
<a name="about-the-project"></a>
## About The Project

<img src="https://raw.githubusercontent.com/patrickvorgers/SPC/main/images/SPC hardware.png">

### Floorheating usecase

Are you using floor heating and struggling with low temperature issues? The Smart Pump Control has the answer! By integrating this intelligent device into your heating system, you can optimize your energy consumption and maintain the perfect temperature in your home.

The Smart Pump Control is designed to work seamlessly with your heat pump and central heating system. It detects when either of these sources is producing heat and then intelligently activates your floor heating pump. This means you no longer have to keep the pump running continuously, wasting electricity when it's not needed. Instead, your heating system operates at its peak efficiency, saving you money on your energy bills.

### Take Control with Home Automation

With the Smart Pump Control, you're gaining more control. You can easily monitor and manage your Smart Pump Control through popular home automation systems like Home Assistant. Adjust settings from the convenience of your smartphone or computer. It's a smarter, more connected way to manage your pump.

### Key Benefits of Smart Pump Control:
<ul>
    <li>Energy Savings: Reduce electricity consumption by only running your pump when necessary.</li>
    <li>Easy Installation: Simple setup ensures you can start saving in no time.</li>
    <li>Standalone operation: A Home Automation system is not required to operate.</li>
    <li>Home Automation Integration: Seamlessly integrate with Home Assistant or other automation systems for remote control and monitoring.</li>
    <li>Multiple forms of activation: Temperature based activation (threshold or delta) but also on external state triggers.</li>
</ul>

### Technical features of Smart Pump Control:
<ul>
    <li>Temperature based activation: Activate the pump based on a temperature trigger (threshold / delta).</li>
    <li>Autorun: Automatically run the pump based on a period of inactivity to prevent damage to the system.</li>
    <li>Frostprotection: Automatically run the pump when the registered temperature it too low to prevent frost damage.</li>  
    <li>WebUI: Fully configure the SPC using a WebUI.</li>
    <li>Full API support: All userinterface functionality is also available as an API.</li>
    <li>MQTT support: Status information can be published via MQTT and used in any system that supports MQTT.</li>
    <li>Home Automation integration: Home Assistant autodiscovery of the device and monitoring and configuration via Home Assistant.</li>
    <li>External Trigger support: Trigger the Smart Pump Control based on an external JSON information. This can be any system that provides JSON data. For instance: Home Assistant or Heat pump systems.</li>
    <li>Multiple devices: Support for multiple SPC's on the same network.</li>
    <li>Firmware update: New firmware releases are automatically detected. Upgrade can be initiated via WebUI and API.</li>
</ul>

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- GETTING STARTED -->
<a name="getting-started"></a>
## Getting Started

Follow these simple steps to setup your Smart Pump Control

<a name="installation"></a>
### Installation

1. In case temperature sensors can be connected, connect the temperature sensors to the device.
1. Plug the device in an electrical outlet and wait for the blue led to start blinking (WiFi accesspoint mode).
1. On your phone connect to the WiFi accesspoint and follow the steps to connect the Smart Pump Control to your WiFi network. It can take some time before the accessportal pops up so please be patient.
    - <b><i>SPC-S-AP</i></b> for the socket version
    - <b><i>SPC-SC-AP</i></b> for the socket version with no temperature sensors (core version)
    - <b><i>SPC-AP</i></b> for the basic version
1. After the Smart Pump Control has been connected to the WiFi, the Smart Pump Control can be accessed via the below links
    - [http://spc-s.local](http://spc-s.local) for the socket version
    - [http://spc-sc.local](http://spc-sc.local) for the socket version with no temperature sensors (core version)
    - [http://spc.local](http://spc.local) for the basic version.
1. On the device page it is possible to rename the device into a more meaningfull name (needed when using multiple Smart Pump Control's on the same network)
1. In case temperature sensors can be connected, identify the temperature sensors by holding a single temperature sensor in your hand and monitor for 30 seconds on the SPC startpage the temperature of the sensors. On the configuration page the identified temperature sensor can be assigned (if needed) to another circuit and/or flow/return role.  
1. Update the configuration to your liking

<a name="restart-reset"></a>
### Restart/Reset

#### Restart

Single press the button on the device. This will restart the device and preserve the configuration.

#### Configuration reset

Double press the button on the device. This will restart the device and reset all the settings to the factory defaults except for the WiFi connection.

#### Factory reset

Press and hold the button on the device for at least 3 seconds. This will restart the device and reset all the settings to the factory defaults including the WiFi connection. After restart the blue led will start blinking to indicate that the device is in WiFi accesspoint mode and that the WiFi needs to be configured.

<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- USAGE EXAMPLES -->
<a name="usage"></a>
## Usage

<a name="temperature-activation"></a>
### Temperature activation

<!-- Image Grid -->
<table border="0" cellpadding="10">
  <tr valign="top">
    <td>
      <h3>Activate when above</h3>
      <img src="https://raw.githubusercontent.com/patrickvorgers/SPC/main/images/Example - activate when above.svg" alt="Activate when above">
      <p>The pump is activated in case the temperature rises above the activation temperature. The pump is turned off in case the temperature falls below the calculated hyteresis temperature (activation temperature - hysteresis).<br><br><b>Usage example:</b><br>Floor heating pump activation when central heating is producing heat.</p>
    </td>
    <td>
      <h3>Activate when below</h3>
      <img src="https://raw.githubusercontent.com/patrickvorgers/SPC/main/images/Example - activate when below.svg" alt="Activate when below">
      <p>The pump is activated in case the temperature falls below the activation temperature. The pump is turned off in case the temperature rises above the calculated hyteresis temperature (activation temperature + hysteresis).<br><br><b>Usage example:</b><br>Boiler heating when the temperature falls below a threshold.</p>
    </td>
  </tr>
  <tr valign="top">
    <td>
      <h3>Activate when &Delta;T above</h3>
      <img src="https://raw.githubusercontent.com/patrickvorgers/SPC/main/images/Example - activate when delta-t above.svg" alt="Activate when &Delta;T above">
      <p>The pump is activated in case the &Delta;T temperature (temperature flow - temperature return) rises above the activation temperature. The pump is turned off in case the &Delta;T temperature falls below the calculated hyteresis temperature (activation temperature - hysteresis).<br><br><b>Usage example:</b><br>Floor heating pump activation when there is a positive temperature difference in temperature between the central heating and the floor (heating during winter). This is usefull in case high and low temperature heating (central heating and heat pump) is mixed and no fixed temperature can be set to activate the floor heating pump.</p>
    </td>
    <td>
      <h3>Activate when &Delta;T below</h3>
      <img src="https://raw.githubusercontent.com/patrickvorgers/SPC/main/images/Example - activate when delta-t below.svg" alt="Activate when &Delta;T below">
      <p>The pump is activated in case the &Delta;T temperature falls (temperature flow - temperature return) below the activation temperature. The pump is turned off in case the  &Delta;T temperature rises above the calculated hyteresis temperature (activation temperature + hysteresis).<br><br><b>Usage example:</b><br>Floor heating pump activation when there is a negative temperature difference in temperature between the central heating and the floor (cooling during summer).</p>
    </td>
  </tr>
</table>

<a name="web-ui"></a>
### Web UI

Main screen showing the state of the pump and temperature sensors<br> 
<img src="https://raw.githubusercontent.com/patrickvorgers/SPC/main/images/SPC config.png" width="75%" height="75%"><br>
Trigger configuration for automatically starting/stopping the pump (autodetection for Quatt devices)<br> 
<img src="https://raw.githubusercontent.com/patrickvorgers/SPC/main/images/SPC trigger.png" width="75%" height="75%"><br>
<img src="https://raw.githubusercontent.com/patrickvorgers/SPC/main/images/SPC trigger1.png" width="75%" height="75%"><br>
24h temperature history including pumpstate<br> 
<img src="https://raw.githubusercontent.com/patrickvorgers/SPC/main/images/SPC history.png" width="75%" height="75%"><br>
Logbook show when the pump was activated<br> 
<img src="https://raw.githubusercontent.com/patrickvorgers/SPC/main/images/SPC logbook.png" width="75%" height="75%"><br>
Configuration tools<br> 
<img src="https://raw.githubusercontent.com/patrickvorgers/SPC/main/images/SPC tools.png" width="75%" height="75%"><br>
Firmware update<br> 
<img src="https://raw.githubusercontent.com/patrickvorgers/SPC/main/images/SPC update.png" width="75%" height="75%"><br>

<a name="home-assistant-ui"></a>
### Home Assistant UI
TODO

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- ROADMAP -->
<a name="roadmap"></a>
## Roadmap

- [ ] Autodetect IP of the external trigger system based on the provided url
- [ ] Different pump activation temperatures for summer and winter
- [X] Default behaviour when the external trigger system is not available (activate pump / deactivate pump)
- [X] Delta triggering, when difference between two sensors is above or below a threshold activate the pump (scenario: difference between flow and return)
- [X] Logbook of trigger events and their duration

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
