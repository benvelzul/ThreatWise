# ThreatWise - Cyber Security LEarning APp

This app is made for the Premier's Coding Challenge and its aim is to help students (from grade 4-10) be able to detect threats (u know like Threat - Wise, hahahahaha) and be more safe online. 


### Key Features

* **AI Chatbot:** A gemini api powered chatbot that only answers to cyber security questions. 
* **Attack Simulator:** A simulater where it looks like an email and u have to read the text closely to spot the threats in the email (over 50k posible solutions)  
* **Password Checker:** A pasword checker that hashes the password u put there and then it calculates
* **Mascot:** Our own mascot just like duolingo help users feel more engaged and it looks cool
* **Courses:** We got a total of 3 courses with quizzes (i had to make AI polish my horrible explanation about the scam spotting so sorry if it sound like AI) 


## Feature description and facts

## ChatBot Challenges with Gemini Flash

Integrating the Gemini Flash API Key into the code proved quite difficult. At first, I had to create a local file called env.json with the API Key inside it, but it could not be comitted to GitHub because it would publically release the key. Later on, we found out that you could create a secret variable in Github, and when deployed, the ChatBot would work perfectly. I gave the ChatBot a systeminstruction to be purely cybersecurity based, which contributes further to the cub security and learning aspect of the project

## Password checker system

The password checker's logic is quite simple, as it calculates the strength bases off of the amount of characters, whether it has upper or lowercase letters, numbers, and special characters. The time system for a computer hacking the password is for interactiveness, and provides a hint to how long a computer may crack the password, but is not completely true. It is based off of the length of the password divided by the hashes per second, and further rounding to the nearest secondor year through mathermatical algorithms. 

### Email and Phishing Scenario Generator

the simulator is made out of components instead of hardcoded emails and thats how it reaches the ginormus amount of possible emails. 

here are the components: 
* **Greeting**
* **Issue**
* **Call to Action (CTA)**
* **Signature**

each one of this components has around 10-30 variations in each difficulty

* Easy
* Medium
* Hard
* Expert

overall, the simulator can generate **approximately 45,000 unique email scenarios**, with a different combination being created each time a user plays. This provides a highly varied experience while making it difficult for players to memorize answers, encouraging them to identify phishing attempts based on the email's content rather than repetition.

### Course Engine

The course engine works by reading .md files that have titles like `### course` or `### quiz` and then the algorythm divides it into course content and questions. 

The course is displayed by using the MarkDown viewer library in flutter making it really easy to display this. 

The question structure in markdown is: 
```md
### Question {num}
{Question Title}
**Difficulty:** {easy, medium, hard, or expert}
**Points:** {points}
- [] Ans 1
- [] Ans 2
- [x] Correct ans 
- [] Ans 4
```
As you can see in the example above the correct ans is recognized by having the cross mark in it. 
and this is divided intro variables in list/dictionary and then you access them and show the Question UI and animations. 

### Animations

The animations made the app completly change its interactivity and look. 
The main animations include the **Confetti**, and the **Sliding animation** on the email simulator. 
The sliding animation had to be coded by scartch but it only took around 2-3 hours to finish and made a really good image. 

The confetti was a lot easier because of the confetti library and it just required some testing but it was done in around 15 minutes. And it took like 5 lines of code and then it generated an amazing feeling and looks. 

## Future Roadmap
If we continue developing this platform, our next steps include:

* **Cyber Trivia Battles**: A local multiplayer mode where students can challenge each other to quick safety quizzes.

* **Live Threat Feed**: A simulated news broadcast pulling in real-world data breaches to teach users about current scams circulating in Australia.

* **Achievement Badges**: Unlockable digital badges as users complete modules to further increase gamification.

* **More courses:** I wanna add more courses but rn im too lazy to do them.
---

## Setup & Installation
To run this project locally, make sure you have the Flutter SDK installed on your system.
1. Clone the repository:
    ```Bash
    git clone [https://github.com/benvelzul/Threat-Wise-Premiers-Coding-Challenge.git](https://github.com/benvelzul/Threat-Wise-Premiers-Coding-Challenge.git)
    cd Threat-Wise-Premiers-Coding-Challenge
    ```

2. Fetch dependencies:
    ```Bash
    flutter pub get
    ```
3. Run the app:

    ```Bash
    flutter run
    ```

But if you just want to test it out here is the link: https://benvelzul.github.io/Threat-Wise-Premiers-Coding-Challenge/ 

---

## Team & Acknowledgments
Developed by:

**Benjamin Velez Zuluaga**

**Zander Setiawan**

Submitted for the Premier's Coding Challenge (QLD).

### Tester Credits

* Sebastyen Nagy 
* Tracey Iki
* Belinda Bretherton 
* Matthew Sutherland
* Rosario Velez Zuluaga
* Tatiana Zuluaga Garcia
* Thiago Servidoni Dominguez
* Alexander Sabariz

### Extra Special Credits 

* Matthew Sutherland - Writer of cybersecurity courses
* Tracey Iki - Coordinator of co-curricular activites

## AI usage

This project used AI to research and understand concepts of cyber security, algorithims, and Flutter (and Dart). And some texts like the README was polished by AI to correct grammar (as you can see in this paragraph no AI polished it) and sound more professional. 
