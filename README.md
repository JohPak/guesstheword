# Guess the Word
**Game gives definition of words and player has to guess the word in question.**
Player is able to buy hints with points (letters and audio) and is given 3 chances to guess each word. The game ends when player has lost all points. Player can also save his/her name and score if new highscore is reached, but it will restart the game.

Guess the Word | Guess the Word | Guess the Word
------------ | -------------| -------------
![Image of Guess the Word](http://jossu.net/guess/1.png) | ![Image of Guess the Word](http://jossu.net/guess/2.png) | ![Image of Guess the Word](http://jossu.net/guess/3.png)




## What is does?

The game uses Merriam-Webster Dictionary API and a txt-list of ~6000 most common english nouns. Each word is drawn randomly from the list and then definition is loaded from the API.

Hints are letters of the word. You can buy as many hints as you have points to. Currently each letter cost -10 points.
Audio hints cost -50 points. Game will look audio from the definition loaded. Not all words has audio available, and this must be checked in the game (not implemented yet).
Audio makes guessing the words a bit too easy, but the price is high compared to points received from guessing word right (+40 p). Audio is added mainly just for fun :)

### Play the game
http://www.jossu.net/guess

### Further development ideas
- Include different API for drawing random word
  - Currently i was unable to find free way to draw a random word to be used in loading the definition. Most APIs require to search items by word and not by random.
  
- Check if audio file is available
  - By default game is offering to buy audio hint fo every word. It is not checking whether there is one available from the API. Therefore player can buy empty audio hint and lose -50 points.

- Make game responsive
  - Game shows correctly only on desktop (perhaps tablet too?)
  
- Use Single File Components, templating etc
  - It's getting harder to read because almost everything is in the same index file
  - I have not used templates
