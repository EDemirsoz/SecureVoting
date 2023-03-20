
# Secure Voting Application

This is basic voting application that uses blockchain to store votes securely, and it allows people to vote from their home since blockchain is used to confirm, it is secure.

##  Disclaimer
The project available in this repository is an academic project and is not intended to be publicly available since it is related to academic coursework, and there is a potential for academic misconduct if it is used improperly. Therefore, only a video recording of the project is available for viewing.

If you would like to request access to code base and additional materials related to this project, please contact me directly and make your request. Please note that access to any additional materials will be granted solely at my discretion and only for legitimate educational or research purposes.

By accessing the video recording of this project, you acknowledge and agree that you will not use it for any unauthorized or unethical purposes, and that any misuse of the project may result in serious consequences, including academic penalties and disciplinary action.
## Tech Stack

- Python


## Installation and Setup

1. First, you need to install docker on your machine in order to be able to run NaiveChain. You can use this link https://www.docker.com/products/docker-desktop to download for free, and after following installation guide, you will see this page on your Docker Desktop application.

![image](https://user-images.githubusercontent.com/64825806/226467564-8d1c5519-8448-4fa9-8c2b-780980a37a75.png)

2. Now you need to clone my repository to your machine in order to be able to use it. For this, I will use Git Bash, but you can use any method that you want for cloning the repository.

	- First, change your directory to where you want to clone this repository. For test purposes, I changed my directory to Desktop.

  ![image](https://user-images.githubusercontent.com/64825806/226467606-2cff338c-b6f0-43b6-95b4-49516314345e.png)

	- Use “git clone repositoryName” command to clone the repository.
	
  ![image](https://user-images.githubusercontent.com/64825806/226467643-4ff74e4e-2667-4c1d-9a46-6291c6c4366c.png)

	- Change your current directory to “repositoryName” and run “docker-compose up” command to run NaiveChain via docker.
	
  ![image](https://user-images.githubusercontent.com/64825806/226467675-e9b8b8fb-60f1-498e-b6cc-ed5521df42ed.png)

	- Now, you will see this on your Docker Desktop application page. This means naivechain and nodes are running.
	
  ![image](https://user-images.githubusercontent.com/64825806/226467706-c77c1138-7735-4370-bfe0-c132bc598871.png)

	- Now, you need to run the NS Voting System application. For this, open new command prompt, and change your directory to “repositoryName\myProgram”, and run “main.py” (I assume you have python installed on your machine, if not then you need to install it).
	
  ![image](https://user-images.githubusercontent.com/64825806/226467732-f35a7a60-dd9f-4d5c-92f0-8d3017fd09f3.png)

	- After this step, you have successfully installed and executed the application. It is ready for you to use it.
	
## Run Locally
In this application, user has 4 options:

1. Vote: This option allows users to vote for one of the candidates.

![image](https://user-images.githubusercontent.com/64825806/226467774-1a02c5a0-37b4-49ca-9787-7ab70604eb70.png)

  * As you can see, there is a list of candidates, and user is prompted to select one of the candidates from list and enter their voterID. If user selects candidate out of range or enters voterID that is out of range or voterID that has already been used to vote, the program will display information message and allow them to make those selections again. Otherwise, will display voterID and voted for which candidate to confirm their vote.
	
2. See Current Results: This option allows users to see total vote count, and the distribution of votes.

![image](https://user-images.githubusercontent.com/64825806/226467805-01637b4e-e571-4931-8d7b-d1b68b868299.png)

	This page displays current vote count to inform voters. They can see instant changes here.
	
3. Get Blockchain (Admin): This option is developed for Admins to see entire blockchain in order to investigate more about nodes and data in them.

![image](https://user-images.githubusercontent.com/64825806/226467832-4f1d6631-a85c-4752-920f-55274f429d36.png)

	Admin can see entire blockchain here, and investigate if something goes wrong. The format of data “VoterID#x#y”, this means x is the votedID and y is the id of candidate that user voted for.
	
4. Exit: This option allows users to exit from the program. It will display good-bye message.

![image](https://user-images.githubusercontent.com/64825806/226467874-9c498ca1-72ee-4143-8468-79f9ef6f214f.png)

