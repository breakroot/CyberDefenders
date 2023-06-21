# CyberDefenders
<div id="top"></div>
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


<!-- PROJECT LOGO -->
<!-- PROJECT LOGO -->
<br />
<div align="center">
  <h1 align="center">CyberDefenders</h1>
  <br>
  

  <img src="https://github.com/breakroot/CyberDefenders/blob/main/l'espion.png/cyberdefenders_og%20copy.png">

<h3 align="center">Project Module - Blue Teaming</h3>
</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
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
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

The Cyberdefenders platform aims to provide users practical experience defending against cyberattacks as a cybersecurity education and training tool. The website is designed for professionals, students, and anybody else who wants to learn more about cybersecurity or advance their knowledge in this field.

There are several tools and functionalities on the Cyberdefenders platform, such as:<br>

● Cybersecurity simulations: The software offers accurate representations of online threats and enables users to practice thwarting them in a secure setting.
<br>

● Learning materials: To assist users in learning about cybersecurity ideas and best practices, the platform provides a variety of instructional tools, including        articles, videos, and interactive content.
<br>

● Programs for certification: Cyberdefenders provides certification opportunities for users to show off their cybersecurity expertise.
<br>

● Support from the community: The site provides a user and mentor community that may help those who are studying and using cybersecurity techniques.
<br>

In general, Cyberdefenders is a thorough platform that offers users a variety of tools and possibilities to study and practice cybersecurity. CyberDefenders allow users to demonstrate their cybersecurity expertise and understanding.


<p align="right">(<a href="#top">back to top</a>)</p>

# 1. L'espion<br>
Category : Threat Intel

According to Crowdstrike, 'Threat intelligence is data that is collected, processed, and analyzed to understand a threat actor’s motives, targets, and attack behaviors. Threat intelligence enables us to make faster, more informed, data-backed security decisions and change their behavior from reactive to proactive in the fight against threat actor.'

In this challenge, a client has asked users to look into the incident and identify the attacker after their network was compromised and taken offline. Currently on the scene and having completed a preliminary investigation are incident responders and digital forensic investigators. Their research demonstrates that the attack was launched from a single user account, most likely an insider.
### Process
Without utilizing a terminal, we will resolve this situation.
After downloading the challenge materials, we will receive a zip file including all the introductory information that can help us with our inquiry.<br>


<p align="center">
<img src="https://github.com/breakroot/CyberDefenders/blob/main/l'espion.png/pass.png"><br>

  
  After extracting the zip file we can see that there are three files. One of them is a text file named "Github". The name of the other two image files are "Office" and "WebCam".<br>

  
<p align="center">
<img src="https://github.com/breakroot/CyberDefenders/blob/main/l'espion.png/info.png"><br>

  
If we open the file named "Github", we can see that the file contains the URL of an certain Github account.<br>

  
<p align="center">
<img src="https://github.com/breakroot/CyberDefenders/blob/main/l'espion.png/git.link.png"><br>

  
The URL address leads us to an github account of the user "EMarseille99". After visiting the github profile we can see that the user has 14 repositories that we can check manually one by one.


<p align="center">
<img src="https://github.com/breakroot/CyberDefenders/blob/main/l'espion.png/github-profile.png"> 


Now let's try to solve some question with the information we already have.

**<h3>Question1</h3>**
<p align="center">
<img src="https://github.com/breakroot/CyberDefenders/blob/main/l'espion.png/qq1.png">


  Our main goal here is to find out the API key added to the respiratories. Since we've checked all 14 repositories one by one, we found something interesting in the repository named "Project Build — Custom-Login-Page". This repository has two files. As soon as we open the "Login Page.js" file, we can see the API key in the code's top-most section. 


<p align="center">
<img src="https://github.com/breakroot/CyberDefenders/blob/main/l'espion.png/q1.png">
  
  * Answer
  ```sh
  aJFRaLHjMXvYZgLPwiJkroYLGRkNBW
  ```
**<h3>Question2</h3>**
<p align="center">

<img src="https://github.com/breakroot/CyberDefenders/blob/main/l'espion.png/qq2.png">


As we scroll down the same file, we can see a base64-encoded password.
<p align="center">

<img src="https://github.com/breakroot/CyberDefenders/blob/main/l'espion.png/q2.png">
Decode it for the answer.<br>
 
 <img src="https://github.com/breakroot/CyberDefenders/blob/main/l'espion.png/q2..png"><br>
 * Answer
  ```sh
  PicassoBaguette99
  ```
**<h3>Question3</h3>**
<p align="center">
<img src="https://github.com/breakroot/CyberDefenders/blob/main/l'espion.png/qq3.png">


Since we previously walked through each repository one at a time, we have encountered a number of frameworks and tools related to crypto-mining. There is also **XMRig**. Open-source software called **XMRig** is made for mining cryptocurrencies like Monero or Bitcoin.. <br>
 <img src="https://github.com/breakroot/CyberDefenders/blob/main/l'espion.png/q3.png">

 * Answer
  ```sh
 XMRig
  ```
By examining the provided github profile, the first three questions have been answered. Now, if we search the insider's username that we copied from github on google, we'll discover that they also have accounts on Instagram and LinkedIn in addition to github.

<p align="center">
<img src="https://github.com/breakroot/CyberDefenders/blob/main/l'espion.png/q4.png"> 

More details about the person are available on their linkedin and Instagram profiles. 


**<h3>Question4</h3>**

<p align="center">
<img src="https://github.com/breakroot/CyberDefenders/blob/main/l'espion.png/qq4.png"><br>

It is evident that the performer for the play attended Sorbonne University.<br>

<p align="center">
<img src="https://github.com/breakroot/CyberDefenders/blob/main/l'espion.png/q4.4.png"><br>

 * Answer
  ```sh
Sorbonne
  ```
  **<h3>Question5</h3>**

<p align="center">
<img src="https://github.com/breakroot/CyberDefenders/blob/main/l'espion.png/qq5.png"><br>

Additionally, we can observe from his or her linkedin bio that they are a member of Steam..<br>

<p align="center">
<img src="https://github.com/breakroot/CyberDefenders/blob/main/l'espion.png/q5.png">

<p align="center">
<img src="https://github.com/breakroot/CyberDefenders/blob/main/l'espion.png/q5.1.png"><br>

 * Answer
  ```sh
  Steam
  ```
 
 **<h3>Question6</h3>**

<p align="center">
<img src="https://github.com/breakroot/CyberDefenders/blob/main/l'espion.png/qq6.png"><br>

The URL to the insiders Instagram profile can be found by visiting the insiders Instagram account.

<p align="center">
<img src="https://github.com/breakroot/CyberDefenders/blob/main/l'espion.png/q6.png"><br>
 
  * Answer
  ```sh
  https://www.instagram.com/emarseille99/
  ```
  
  **<h3>Question7</h3>**
  
  <p align="center">
<img src="https://github.com/breakroot/CyberDefenders/blob/main/l'espion.png/qq7.png"><br>
 
 He or she uploaded a picture of the location they visited over the holiday to insiders' Instagram account.

<p align="center">
<img src="https://github.com/breakroot/CyberDefenders/blob/main/l'espion.png/q7.png"><br>
 
 We can reverse image search this picture.<br>
 
<p align="center">
<img src="https://github.com/breakroot/CyberDefenders/blob/main/l'espion.png/q7.1.png"><br>
 It is a picture of the stucture Marina Bay Sands which is in Singapore.
    
   * Answer
  ```sh
  Singapore
  ``` 
  
  **<h3>Question8</h3>**
   <p align="center">
<img src="https://github.com/breakroot/CyberDefenders/blob/main/l'espion.png/qq8.png"><br>

 "Nice to meet friends & family Photo 1/2" was the caption on 2 photos that The Insiders uploaded on Instagram. A UAE flag can be seen in the back in the first image.<br>

 <p align="center">
<img src="https://github.com/breakroot/CyberDefenders/blob/main/l'espion.png/q8.png"><br>
  
  So the country of inser must be UAE.<br>
From the second picture we can see Burj Khalifa in the back. 
   
<p align="center">
   <img src="https://github.com/breakroot/CyberDefenders/blob/main/l'espion.png/q8.1.png"><br>
     
Search this image in the google.
   
  <p align="center">
   <img src="https://github.com/breakroot/CyberDefenders/blob/main/l'espion.png/q8.2.png"><br>
    
 we can see he city insiders family live is **Dubai**
     
   * Answer
  ```sh
  Dubai
  ```
**<h3>Question9</h3>**

<p align="center">
<img src="https://github.com/breakroot/CyberDefenders/blob/main/l'espion.png/qq9.png"><br>
  
  <p align="center">
<img src="https://github.com/breakroot/CyberDefenders/blob/main/l'espion.png/office.jpg"><br>
  
  Reverse image search this.
  
  <p align="center">
<img src="https://github.com/breakroot/CyberDefenders/blob/main/l'espion.png/q9.png"><br>
    
    The structure in this image is clearly the entrance of Birmingham New Street Station.
    
   * Answer
  ```sh
  Birmingham
  ```
    
**<h3>Question10</h3>**

<p align="center">
<img src="https://github.com/breakroot/CyberDefenders/blob/main/l'espion.png/qq10.png"><br>
  
<p align="center">
<img src="https://github.com/breakroot/CyberDefenders/blob/main/l'espion.png/WebCam.png"><br>

We have this webcam image from EarthCam to answer your final query. Use a reverse image search on this image to quickly solve this.
    
 <p align="center">
<img src="https://github.com/breakroot/CyberDefenders/blob/main/l'espion.png/WebCam.png"><br>

Now if we search where University of Notre Dame is located which is **Indiana**.

<p align="center">
<img src="https://github.com/breakroot/CyberDefenders/blob/main/l'espion.png/q10.1.png"><br>

   
   
   * Answer
  ```sh
  Indiana
  ```   
