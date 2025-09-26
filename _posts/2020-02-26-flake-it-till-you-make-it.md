---
layout: post
title: 1.4 Lab 1
subtitle: Digimon Dataset
cover-img: /assets/img/path.jpg
thumbnail-img: /assets/img/thumb.png
share-img: /assets/img/path.jpg
tags: [books, test]
author: David Hutchinson
---

1.What is the average speed (Spd) of all Digimon?
To answer this question I first created a nested dictionary, storing each Digimon's data using their numbers as the key. I then added all of the Digimon's speed and counted them so that I could find the average speed and print it. ![avg-spd](https://beautifuljekyll.com/assets/img/avg_spd.jpg)

2.Write a function that can count the number of Digimon with a specific attribute. For example, count_digimon("Type", "Vaccine") would return 70. 
For this question I created a function to count the Digimon by a specific attribute and value. I had a bit of trouble with this one but with the help of copilot and using the itertools module I was able to complete it with this function:
![question-2-function](https://beautifuljekyll.com/assets/img/question2.jpg)
In this function you are able to search through an attribute like "Type" and count the number of digimon with a specific type.

3.The Digimon on your team are restricted by the total amount of Memory that they need. If your team only has 15 Memory, name a team of up to 3 Digimon that has at least 300 attack (Atk) in total.
![question-3-function](https://beautifuljekyll.com/assets/img/Question3.jpg)
This question gave me the most trouble however I found that using the itertools module was the easiest way of answering it. The outer loop (size in range(1, team_size + 1)) checks teams of size 1, 2, and 3. and the For loop with itertools.combinations(candidates, size) generates all possible unique teams of the given size. For each team, it sums up the memory and attack values. If the team meets the requirements, it returns a list of Digimon names in that team.
![final-result](https://beautifuljekyll.com/assets/img/Result.jpg)
In the end this Lab was a great learning experience.