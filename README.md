Download Link: https://assignmentchef.com/product/solved-cs-assignment-4-containers
<br>
You will make a program to run a tournament.  Start with your assignment 3 program for creatures if possible.  If you had issues with assignment 3 and need to begin fresh, reference the creature descriptions from assignment 3 to build your fighters.  A user will enter the number of fighters both players will use.  The first player supplies a lineup of creatures in order.  The second player then supplies their lineup of creatures in order. After each round you will display which type of creatures fought and which won.   At the end of the tournament your program will display: the first, second, and third place finishers, their teams, as well as which side scored more points.  You will provide an option for the user to see a list of the final order of all fighters (this means you will display the loser pile after displaying the first three finishers).




You should be using polymorphism and all creatures will inherit from the Creature class.  The user should enter the type of creature and name.  You may need to add name or some ID to distinguish 5 Barbarians in a tournament.    Each object should be instantiated and put into their lineup.  You will only use pointers to creatures in your program.  A creature pointer can then be used to indicate an object of a subclass and polymorphism will ensure the correct function is called.  As your TA if you are uncertain what this means.

By lineup I mean something like a batting order in baseball or softball. The head of each lineup fights.  The winner gets put at the back of his team’s lineup; the other goes to the container for those who lost.  The lineup order cannot be changed once the players are entered.  Similarly, the loser pile should have the last loser at the top and the first loser at the bottom.

NOTE:  Depending upon how you implemented the fight in Assignment 3 you could have ties.  How does that tie change your end of match logic?  What do you do if the final match is a tie?  Specifically, where do you put the fighters? JJ

For this program you must use the structures from Module 1 to hold the lineups and the loser pile. Which (stack-like or queue-like) will you use for the lineup?  Which will you use for the loser pile?

Even if a creature wins she may have taken damage.  You should restore some percentage of the damage when they get back in line. Make this simple as you are adding a new member function to the parent class.  Some examples are: generate a random integer in some range, or on a role of 5 they recover 50% of the damage they lost, or some scheme of your own.   If you want to use a different recovery function for each character that is fine.  Remember to use polymorphism if the recovery is different for different creatures!

A special ability may find a creature stronger than when they started!  If they ended a round with more strength (hit points) than they start with it is reset according to the table in Assignment 3.  If a special ability could only be used once, it is also reset.

At the end of the tournament you should display the first, second, and third place finishers.  You should also indicate their team(s), and which team won the tournament.  This is another element you must define in the analysis and design stage. You must have a method to determine the winner:  the total points for each team?  The win-loss. Record?  If a weaker creature beats a stronger creature maybe they get more points? JJ  The losers are sorted (most recent first) in the loser pile.  Can you use that information?  In your final design document clearly state the system you are using and how you will implement it.

This is a programming assignment and not a complete game!  Other than entering the lineup the players just wait for the results.  They may take no further actions.  Make sure you test your program with instances of all creature types you’ve created. You may not be able to do an exhaustive test but make it as extensive as you can.