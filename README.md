Lab 1:  Setting Up Your First Website
OBJECTIVES
This lab will introduce you to setting up your own website using a GitHub repository deployed to a GitHub Page. You will also be introduced to Git and the open-source integrated development environment (IDE), Atom. The four tasks for this lab are:
1.	Setting Up Your GitHub Account
2.	Setting Up Your First Repository and GitHub Page.
3.	Introduction to Git, a Distributed Version Control System
4.	Introduction to Atom and the Hyper-Text Markup Language (HTML)
5.	Add Your Professor and Lab Instructor as Collaborators
 

Task 1. Setting Up Your GitHub Account
GitHub is an online development platform that allows individuals and organizations to host and review code, manage projects, and build software.  There are currently more than 36 million developers subscribed to GitHub with projects ranging from individual open-source initiatives to organizational projects which have hundreds of contributors and thousands of files.  As discussed in the lecture there are three necessary components for a website: 
1.	The code/scripts you use to compile the website (text, pictures, video, downloadable content, etc.).
2.	A web server to host your website.
3.	A domain name, which is a unique URL address that points users to your website.
We will maintain a copy of our codes/scripts on a portable USB drive.  Windows 10 will allow us to open and test any webpage that we create in this lab, without installing any additional software.  GitHub pages will provide us a domain name at yourusername.github.io.  Optionally, GitHub also provides an option for you to use your own domain name www.yourdomain.(com, net, io, etc.).  GitHub even offers simple, fast, and free hypertext transfer protocol secure (HTTPS) encryption which improves the security and privacy of your website.  For example, when you browse a website via HTTPS, it prevents your internet service provider (ISP) from seeing which individual web pages you are viewing, HTTP does not offer this protection.

Sign-up for Github:
1.	Navigate to Github.com and sign up for an account using the form provided on the homepage. 
2.	GitHub will send an email to you, make sure you “Verify email address” using that email.
3.	If asked, complete the verify test to prove that you’re a human.


Optional GitHub Student Developer Pack
If you would like to, GitHub offers a “GitHub Student Developer pack”, it is a digital collection of open-source software, discounts, and some paid tools (IE. A GitHub Pro account).  You can set this up later by going to https://education.github.com. 

For now, let’s continue with Step 4.

4.	Leave the green checkbox selected for a free account, make sure you don’t leave any boxes checked that you don’t want (ie. “Send me updates on GitHub news, offers, and events).  Then, click “Continue”.  At your own discretion, fill out the next step in the sign-up process or skip it.  Then, you will be brought to a page to verify your email address, if you have not already.  Go ahead and get that done!

Task 2. Setting Up Your First Repository and GitHub Page
Now, it’s time to setup a repository to host your website.  Most of the following instructions were taken from https://pages.github.com and adjusted/sorted to facilitate learning outcomes for this assignment.
1.	After signing into GitHub.com, at the top-right hand corner you should see an auto-generated icon with a down-arrow beside it.  Click it and then select “Your repositories”. 
2.	Click “New”.  
3.	In other situations, you could name your repository uniquely to identify it’s purpose.  However, for this task, it is required that you name the repository, username.github.io, where username needs to match your username exactly as it appears.  
4.	Take note of the option to add a “.gitignore”, we don’t need it at this time, but in the future we will use this to hide sensitive information, such as files containing Application Programming Interface (API) keys.  Click “Create repository”.
5.	You should have been directed to a page that has options for how to use Git.  Because this is our first time, we will use the command line instructions when completing Task 3.

Task 3. Introduction to Git, a Distributed Version Control System
Linus Torvalds is the person who developed Linux and he is also the creator of Git, if you are looking for a meaning, or acronym to associate with Git, don’t… The word “git” is offensive English slang meaning, “a stupid person”.  When asked about why he named this product “Git”, Linus said “I’m an egotistical bastard, and I name all of my projects after myself.”  With that said, let’s continue setting up our site and let’s learn about how we will use Git, a distributed version control system.
1.	On your computer, open the program, “Git Bash”.
2.	This window appears to be identical to what you would see when opening a terminal on a Linux operating system.
 
3.	This terminal operates in the same way as a Windows Command Prompt.  Here are a few commands that we will use:
a.	ls 				Lists the contents of a directory.
b.	cd					Changes directory to the location specified.
c.	mkdir				Creates a directory with the name specified.
d.	git clone			Used to clone a repository from GitHub.
e.	echo				Writes text to a specified location.
f.	git add				Moves files to a “Staging Area” to be committed.
g.	git commit			Commits the files for pushing to your repository.
h.	git push			Sends files to the repository.
4.	If you have not, now is the time to plug in your USB drive.  Identify the letter that is assigned to your USB drive.
5.	From the terminal, type the following commands:
a.	cd G: (Replace “G” with the letter assigned to your drive.)
b.	mkdir web_mapping
c.	cd web_mapping
6.	Now, type the following command replacing username with your username:
 
7.	Change directories and create your first html file using the echo command:
 
8.	Finally, we will add, commit, and push the changes that we made:
 
9.	You should see a prompt to enter your login information, enter your username/password and click Login.  It will take about 10 minutes for GitHub to finish setting up your domain after the initial push.  After this, it should take less than a minute for any additional pushes.


Task 4. Introduction to Atom and the Hyper-Text Markup Language (HTML)

Just because your domain is not ready yet, it does not mean that you cannot continue to work on the repository and push new contents to it.  Let’s learn about Atom and continue working on our website.
1.	From the Git Bash terminal use the command “atom .” to open your GitHub website project in Atom, a text editor with interface development environment (IDE) capabilities. 
2.	In the “Welcome Guide” tab, there is an option to “Open a Project”, use this option and navigate to the folder that you created on your USB drive called “username.github.io”.
3.	Here is a simple breakdown of the screen:
 
4.	First, let’s close some tabs that we don’t currently need.  Hover your mouse ove the word “Welcome” at the top-left hand corner of the screen and click the “X” to close it.  Then, do the same for “Welcome Guide”.  The Default Welcome screen area should now have watermark text that displays a tip.  For fun, you can click the “Atom” icon on your task bar to minimize and restore the Atom window, it will show a new tip every time.
5.	Now, double-click index.html from the tree view so that we can edit it.  On the left-hand side are line numbers “1”, “2”.  Also, you can see the text that we created using the echo command “Hello World”.
6.	First, let’s open the “index.html” file in a browser by using the hotkey combination “Ctrl + Shift + B”.  The file says Hello World in the body, and the tab repeats the text that is in the address bar.  Close the browser.
7.	Add HTML tags to your code, make your code look like the code on the right which contains some of the most common HTML tags used in almost every website, then use the hotkey combination “Ctrl+S” to save the file.
8.	Underneath “Unstaged Changes”, click on “index.html” to see changes which were made to the file.  It should look something like this:  
 
9.	Click “Stage File” (top-right), this is the same as typing “git add index.html” in the Git Bash terminal.  “index.html” moved from “Unstaged Changes” to “Staged Changes”.
10.	Where it says “Commit message” in the Git Tab, type “Added HTML tags”, then click “Commit to master”.  After this, “Added HTML tags” will appear above “Initial Commit”.  You can see your user icon to the left of the commit message, and a timestamp to the right of it.  
11.	The last step is to click push the new content to the repository by click the “Push” button.  It is located at the bottom of the screen on the Atom status bar, look below the Git tab for this button  . Now it’s time to open https://username.github.io in your browser, replacing username with your username, of course.  With the <title> tag being used, instead of repeating the address bar text in the tab or on the title bar, it should now say “Hello World Title!”.  If changes have not been loaded yet, just wait a minute or two and refresh.  There is what can be thought of as a “time to live” (TTL) delay for GitHub pages to load any changes made in your repository.


Task 5. Add Your Professor and Lab Instructor as Collaborators
The real beauty of Git and GitHub is in it’s proliferation of open-source community collaboration and a great way to truly take advantage of a decentralized versioning system and GitHub is to collaborate with others.  In this task you will learn how to add collaborators (users with push access) to a repository.  Users with push access are granted push access to the repository, meaning that they can make changes to it.
1.	In your browser go to “github.com” and log in if you are not logged in.  From the home screen there is a link to your GitHub Pages repository on the left-hand side, open it.  If you are not at your home screen, you can click the black and white GitHub cat icon at the top-left hand corner to get there. 
2.	Click the “Settings” tab, and then click “Collaborators from the left-hand menu.
 
3.	One at a time, add the following users: 
DavidAMills
YihongYuan19
 
HOMEWORK ASSIGNMENTS
(10 points)
1.	Create a word document and put a link to your GitHub Pages website at the top of it.  Verify that the link works, if the link does not work, you will not get credit.

(15 points)
2.	In the same document, skip one or two lines and answer the following 3 questions. Only use information that is explained in the tasks above to answer the questions, do not expand on the answers using Wikipedia or any other sources.  It is okay for the answers to be brief (one or two sentences).  Write in complete sentences, answer that are not in sentence form will not get credit.:
What is Git?
	What is Atom?
What is GitHub?

(25 points)
3.	Find, explore, and evaluate two websites that you consider to be examples of web mapping. You are required to provide a general assessment of the user experience, as well as the strengths and weaknesses of each website. Your evaluation must address the following characteristics of each web mapping application: 
	What is the primary purpose of that web mapping application? (If the primary purpose is unclear, comment on the lack of clarity.) 
	What GIS functionality does that application offer? (e.g. geocoding, shortest path, type of spatial analysis) 
	For whom was that application designed? (E.g. researchers, policy makers, general use) 
	How intuitive is the user interface of the application? (i.e., Please describe your personal user experience when exploring the application.) If you were asked to re-design the web mapping application, what would you change? (If you think the application is perfect enough, then justify why you would not change anything.) 
Include the URL of each website, the name of the agency, department, or individual that developed the web mapping application, and a screenshot of the user interface for each evaluation. 

(50 points)
4.	 In this section we will edit our index.html from a “Hello World!” page to one that begins to resemble a resume site.  The comments in the HTML file will introduce you to Cascading Style Sheets (CSS).
1)	Go to:
https://github.com/AnotherAwesomeUser/AnotherAwesomeUser.github.io 
Download the index.html file and the “images” folder to your GitHub pages repository located on your USB drive (overwrite the index.html file you created in the lab).
2)	Use Git Bash to go to your USB drive repository and open Atom as you previously did in Task 4.
3)	Replace the photo of me with a photo of yourself, or of something other than me that you appreciate.  The only requirement for the photo is that it is exactly as wide, as it is tall (IE. 500px by 500px, 750px by 750px, or any other size that has equal width and height.)
4)	Read the comments in the document and edit index.html as follows:
a)	Between the opening HTML tag <div id=”about_me”> and the closing HTML tag </div>, replace the paragraph with one about yourself.
b)	Undergraduate Student Bonus (10 points)/Graduate Student Requirement:
i.	Uncomment the “research_interests” <div> element.
ii.	Replace the text with a paragraph about your research interests.
iii.	In the style sheet create a selector that places the “research_interests” div element 10px from the left-side and 510px from the top.  All other properties in the selector should be the same as in the “about_me” selector.
5)	Save the index.html fil stage each of the Unstaged Changes, commit the Staged Changes with the commit message “Assignment 1 homework” and push the contents to your GitHub page repository.

Deliverable: Submit a word document with the link to your GitHub page, the answers to the homework questions, and the two web map assessments.

Due Date: 5 PM, September 9th, 2019	
