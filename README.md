# Ants vs. Some-Bees

This module is a simple turn-based tower-defense game played on the command-line, completed as part of a [course](http://arch-joelross.rhcloud.com/) at the UW ISchool. 

The below questions should be answered (in detail!) regarding your submission!


##### 1. Spend some time reading through the provided code _carefully_ to make sure you understand it. After you've read the code, in the space below list any _design patterns_ we discussed in class that you can find (note that you may need to revisit the code after each lecture). Be clear about which pattern is used, where, and _why it is being employed_.
> After reading through the code, I noticed that the factory method pattern that was dicussed in lecture was used to create the Ant Colonies and Bee Hives in the game. The Factory method lets a class defer instantiation to subclasses. The factory method pattern is used in this case because we are creating different products of the same type.

##### 2. After you've read the code, is there anywhere that it could be re-architected (e.g., using design patterns) to be more changeable or reusable? 
> After reading through the code, a design pattern that could be used to re-architect the program to be more changeable or reusable would be to implement the strategy design pattern. This would be particulary useful for all the different classes of ants that we are requrired to make. By using this design pattern we wont have redundancy in our code.


##### 3. The tunnels in the `AntColony` are structured as a ___Linked List___ (where each element is a `Place`, and the `exit` and `entrance` variables are the traditional `next` and `prev`). Why is this data structure appropriate (as opposed to, say, an array). _You may need to revisit your notes from CSE 143._
> The tunnuels in the Ant Colony are structured as a Linked List over an array structure because in this assignment we want the tunnels to be able to connect. The Linked List allows this, while arrays dont.

##### 4. Describe the overall architecture you used to implement the different components of this assignment. Did you use inheritance? A particular design pattern?
> When creating the the different kind of Ants, I mainly used inheritance to implement all of them. All of the different subtypes would inherit all of the same qualities from the Ant class. 


##### 5. Specifically, discuss your use of object-oriented design patterns in your program. What patterns did you use in your implementation (be specific)? Why? Is there anywhere you explicitly decided _not_ to use a pattern (e.g., because doing so would have made it more difficult to change the code later, etc)? Be detailed---you should reflect carefully on your own design and architecture work!
> In my program I was able to use the Strategy pattern to implement the watersafe feature. This water safe feature is only used by the scuba ant since it has the scuba gear, it can breathe in the water. It is the only ant that can survive in water, using this pattern allows the behavior to be interchangeable and reusable throughout the program. 
This was the only design pattern I used throughout the assignment, I relied mostly on inheritance fromt the Ant class since most of the subclasses have many of the same features. 


##### 6. Approximately how many hours did it take you to complete this assignment? #####
> It took over 24 hours to complte this assignment.


##### 7. Did you receive help from any other sources (classmates, etc)? If so, please list who (be specific!). #####
> I did not recieve any help from any other sources on this assignment. 


##### 8. Did you encounter any problems in this assignment we should warn students about in the future? How can we make the assignment better? #####
> I didnt' encounter any specific problems in this assignment but it was a difficult assignment for me and in the future maybe have an example ant to implement in class to help students when working on the assignment at home. 

