# brackets
Bracket Creator and formatter


Description:
Create a Python program that generates a tournament bracket for a pickleball tournament. The program should be able to handle different numbers of players or teams and create a single-elimination bracket.

Features:

Number of Players/Teams: Allow users to input the number of players or teams participating in the tournament.
Seeding: Implement a seeding system where higher-ranked players/teams face lower-ranked ones in the early rounds.
Bracket Generation: Based on the number of participants, generate a single-elimination bracket. Ensure that the bracket is balanced and follows standard tournament rules.
Display: Display the generated bracket in a readable format. You can use text representation initially and later consider a graphical representation using a library like Tkinter.
Winner Advancement: Implement a mechanism for updating the bracket as the tournament progresses. Record winners and update the bracket accordingly until a final winner is determined.
Save and Load: Allow the user to save the tournament bracket to a file (e.g., using the pickle module) and load it later.
Bonus Features:

Double-Elimination Bracket: Extend the program to support double-elimination brackets, where a team must lose twice before being eliminated.
Team Names: Allow users to input the names of players or teams for a more personalized experience.
Interactive Bracket: Create an interactive GUI where users can click on matchups to input winners, and the bracket updates dynamically.
Random Seed Generator: If users don't want to input specific seedings, implement an option to randomly seed the players/teams.
Score Tracking: If you want to add an extra layer of complexity, integrate the score tracking system from the previous project to keep track of scores during each match.
