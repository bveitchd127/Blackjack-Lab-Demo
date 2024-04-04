## Description
A card game where players try to get as close to 21 points as possible without going over. This program uses images drawn with text characters, called ASCII art. American Standard Code for Information Interchange (ASCII) is a mapping of text characters to numeric codes that computers used before Unicode replaced it. The playing cards in this program are an example of ASCII art:

You can find other rules and the history of this card game at [this link](https://en.wikipedia.org/wiki/Blackjack).

## How It Works
The card suit symbols don’t exist on your keyboard, which is why we call the chr() function to create them. The integer passed to chr() is called a Unicode code point, a unique number that identifies a character according to the Unicode standard. Unicode is often misunderstood. However, Ned Batchelder’s 2012 PyCon US talk “Pragmatic Unicode, or How Do I Stop the Pain?” is an excellent introduction to Unicode, and you can find it at https://youtu.be/sgHbC6udIqc/. Appendix B gives a full list of Unicode characters you can use in your Python programs.

## Explore
After running the source code a few times, try making experimental changes to it to see how it affects the outcome of the code. 

## Exploration Questions
In the code, identify *three* python functions that you don't recognize. For each unknown python function do the following:
   - Write the line of code and the line number.
   - Before looking it up, try and figure out what it's supposed to be doing.
   - Look it up and in your own words, describe what the functions does more generally.



## Analysis Questions
When applicable, refer to line numbers to be specific.
1. How can you make the player start with a different amount of money? (Refer to line numbers to be specific)
2. How does the program prevent the player from betting more money than they have?
3. How does the program represent a card's suit (what data type)?
4. How does the program represent a card's rank?
4. How (and where) does the program deal with the face cards? (jack, queen, king)
5. How does the program represent a single card?
6. How does the program represent a hand of cards?
7. What do each of the strings in the rows list (created on line 197) represent?
8. What happens if you delete or comment out random.shuffle(deck) on line 148? (You'll need to play a few hands to be confident)
9. What happens if you change money -= bet on line 112 to money += bet?
10. What happens when showDealerHand in the displayHands() function is set to True? What happens when it is False?

## Extensions:
If you finish early, a great exercise is to start with a project and add new features or improve features already in the project.
- If the first two cards have the same value, a player can split them into two hands and wager on them separately. 
- If the player receives a “blackjack” (the ace of spades and a black jack) for their first two cards, the player wins a ten-to-one payout.