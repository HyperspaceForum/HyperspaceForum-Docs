<p align="center">
	<img src="./hyperspacelogoicononly.png" alt="logo" width="50">
	<br>
	<br>
	<img src="./hyperspacelogotextonly.png" alt="logo" width="400">
	<br>
	<br>
Combatting phishing utilizing Large Language Models (LLMs) to remove the "victim" from the equation.
<hr>
</p>

### Why?
Our project is attempting to investigate an innovative approach to combatting internet scams and phishing.
Phishing is an evergrowing attack vector that is costing companies hundreds of millions of dollars every year.

### How?
This small-scale test is intended to serve as a preliminary test to determine the feasibility of this approach. This is being conducted by deploying a website that is disguised as a crypto forum (and is populated with bots). The forum's true purpose is to lure in potential threat actors and entice them to begin attempting to scam users on the forum (Crypto was chosen for its money-driven nature). At this point we (the site admins) can specifically choose to begin targetting the attacker this is done through two main steps. <br>
1. Elimnate the risk to possible real users of the forum by shadow banning the post from everyones feed except for admins
2. Engage the attacker with the LLM this is done by the admin initiating a conversation with the user utilizing the LLM thus starting the back and forth between the two
<br>

### Technical Implementation
Our forum is structured to optimize the ease of interaction between our AI driven admin panel and the site itself this allows us to quickly add new AI features on the fly. We are running a **Flask** webapp which then hooks into **FastAPI** to facilitate the interaction between the AI and the actual site itself (the interaction point being the admin panel). All of our data is stored in a standard MySQL relational database.

All the above is integrated together into the system diagram shown below.

#### Architecture
<img src="./WebpageServerArchitecture-light.png" height="650px">

#### Challenges and Solutions

INPUT CHALLENGES AND SOLUTIONS HERE

### Getting Started
#### Requirements
    - Docker

#### Deployment

To deploy a new instance of the website simply run the commands in order:

```
./buildDocker.sh
./runDocker.sh
```

This will build and then subsequently run a container serving the webroutes on port http://localhost:5000

### Results
 
Link to Site: https://hyperspace.forum/ <br>


### Our Team

**Capstone Team**<br>
Hayden Burgess (AI Integration) ([burgessh@oregonstate.edu](mailto:burgessh@oregonstate.edu)) <br>
Alexander Johnson (Frontend Developemnt) ([johnsa33@oregonstate.edu](mailto:johnsa33@oregonstate.edu))<br>
William Richards (Backend Architecture) ([richawil@oregonstate.edu](mailto:richawil@oregonstate.edu)) <br>

**Project Management**<br>
Isaac Hathaway ([isaac@hathaway.llc](mailto:isaac@hathaway.llc))
