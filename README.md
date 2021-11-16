# Uno_Game_Code_Snippets
## Disclaimer
The contents of this repository hold code snippets of an Uno Game milestone done in Java. In a separate folder is snippets of certain functionality running, such as a +4 being placed down, reversing the flow of the game, etc. Due to GCU policy, I can not create public GIT repositories for milestones/assignents. If you would like to see the full code, please contact me at jacobg43@cox.net. The content below is from the readme.md from the Uno Game repository, which explains the milestone more in depth.
 
 ## Dates of Importance
The Milestone creation took place from January - April, 2021.
It was refactored during October - November, 2021.

## Summary
The creation of an Uno game between four bots was the milestone project for Java I at GCU. The objective was to create a functioning Uno game where four players could take cards from a deck and place them down accordingly (in accordance to card color, value, and/or functionality), and giving the cards the correct functionality. I further enhanced the project by adding additional logic to give the bots more human tendency/strategy (placing cards down with a purpose).

## Strategy
The strategy added to the game was one to simulate what real people would likely do.
If the next players hand is low, then the current player will try to use any card they have to prevent them from advancing. Which card they'll place down depends on what they have
The level of importance is as follows:
- Plus Four
- Plus Two
- Skip
- Reverse

If the next player is not low on cards, then the current player will try to not use any tactical cards. Their next level of importance is as follows:
- numerical cards, matched by color or value
- reverse
- skip
- plus two
- wild card (This ensures that they save a wild card for when they have no cards that match the value or color of the current card)
- +4 (Like the wild card, this is saved last in case they have no cards left and so that if the next player is low, they have this one saved)

## Concepts Demonstrated
The Uno games demonstrates encapsulation and HAS-A relationships. Both the deck and player has cards, demonstrating an aggregation relationship with the player (the player can exist without the cards), while the deck has a composition relationship (the deck needs cards to be itself).
