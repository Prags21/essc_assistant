# ESSC Virtual Assistant
It is a chatbot used for answering common students' queries.
### Engineering Student Success Center, SJSU (ESSC)
ESSC helps students throughout their engineering journey. They do Major advising, hold removal, transfer equivalency petitions and more. They also have workshops for helping students with their job search, resume writing and more.

## Purpose

The center experiences high influx of students asking similar questions most of the time.
It is wise to save time and resources spent on these tasks by having a system that automates such tasks.
Further, students would also have 24X7 access to it so they won't have to wait for a real person to get answers of these  questions.



## Contents

This bot is capable of understanding a total of 23 user utterances.
It has few rules and 3 multi turn interactive stories. It also has few stories that focus on small talk.

Future implementations can expand the chatbot's ability to answer a diverse range of topics. It can be done by having more intents and data (related to the questions that students ask). 
However, the current implementation fulfills the scope and goal of the project.

## Capabilities
This bot can provide the user with the following information when prompted:

1. Collect and store a user's name.

2. Help students with change of major process

3. Students can also inquire about their major advisor.

4. Gives students an overview of ESSC and also give them information about the working hours.

## Implemented Conversation Flows
#### Example 1:
```python
User ->  hi
Bot -> Hey! How are you?
User ->  great
Bot -> Great, carry on!
       How may I be of assitance?
User ->  Who is my major advisor
Bot -> What is your major? 
User -> Select 1: CMPE (CMPE)
Bot -> For CMPE, the advisor is Monica Serna.
       For further help, feel free contact us.
       Bye! Have a great day!
```

#### Example 2:
```python
User ->  i need help
Bot -> Please enter your name
User ->  Pranav
Bot -> Pranav,How may I be of assitance?
User ->  I want to change my major
Bot -> The change of major application process for college of engineering depends on the number of earned units you have
(If you do not know how many earned units you have, check your transfer credit report).
Please select one which applies to you: (Use arrow keys)
 1: If below 60 units (below_60units)
 2: If 60 units or above (above_60units)
   Type out your own message...
User -> Select  1: If below 60 units (below_60units)
Bot -> If you have less than 60 units then please follow the procedure mentioned on this link- https://www.sjsu.edu/essc/coe-undergraduate-advising/change-major/below-sixty-earned-units.php
Did that help you?
User ->  yes
Bot -> Great, carry on!
What can I help you with?
User ->  will my change of major application be accepted?
Bot -> Due to impaction, admittance is not guaranteed and will depend on the capacity of the major. Strive for the highest GPA possible in the prerequisite courses necessary to apply for the major. Also, you are allowed to apply twice for a major.
For further help, feel free contact us.
User ->  bye
Bot -> Bye! Have a great day!
```


#### Example 3:
```python
User ->  hi
Bot -> Hey! How are you?
User ->  good
Bot -> Great, carry on!
Is there anything I can help you with?
User ->  who are you
Bot -> I am an ESSC virtual assistant, powered by Rasa.
User ->  what is essc
Bot -> At Engineering Student Success Center,we help students throughout their engineering journey.We do Major advising, hold removal, transfer equivalency petitions and more.We also have workshops for helping students with their job search,resume writing and more.
User ->  when is it open
Bot -> We are now open. You can schedule appointments via Spartan Connect or you can come to our drop-in hours which is from 11:00am to 12:00pm and 1:00pm to 2:00pm.
We are also available on zoom. You can schedule virtual appointments or you can come to our virtual drop-in hours. Please find the virtual drop-in timings here.
User ->  thanks
Bot -> Bye! Have a great day!
```
These examples illustrate the  conversations flows implemented in this chatbot.
## Notes
In order to run this program, install all the packages in the requirments.txt. This will ensure that the correct versions are loaded. Additionally, it is crucial to note that the chatbot is applicable for SJSU engineering undergrad students. It has various limitations as of now so requires a user to follow the mentioned conversation flow. The name of the user also has limitations. It detects few of the names correctly while others do not have good accuracy.