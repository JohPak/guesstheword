# guesstheword
Game gives definition of words and player has to guess the word in question.
Player is able to buy hints with points (letters and audio) and is given 3 chances to guess each word. The game ends when player has lost all points. Player can also save his/her name and score if new highscore is reached, but this will restart the game.

---

The game uses Merriam-Webster Dictionary API and a txt-list of ~6000 most common english nouns. Each word is drawn randomly from the list and then definition is loaded from the API.

Hints are letters of the word. You can buy as many hints as you have points to. Currently each letter cost -10 points.
Audio hints cost -50 points. Game will look audio from the definition loaded. Not all words has audio available, and this must be checked in the game (not implemented yet).
Audio makes guessing the words a bit too easy, but the price is high compared to points received from guessing word right (+40 p).



### Further development ideas
- Include different API for drawing random word
  - Currently i was unable to find free way to draw a random word to be used in loading the definition. Most APIs require to search items by word and not by random.

- Make game responsive
  - Game shows correctly only on desktop (perhaps tablet too?)
  
- Use Singel File Components
  - Now almost everything is in the same index file
