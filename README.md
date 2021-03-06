# Codenames
Codenames "spymaster" bot

Update: Putting this project on hold for a while. It's fun and very complicated but, for both of those reasons, immensely time-consuming.
This was definitely a larger project than I anticipated or budgeted for, 
but I hope to post the more complete version as soon as I've had more time to spend ironing out the algorithm and cleaning up the code.

gameboard.py
This file contains the code to define and interact with the game components:
1. Creates and stores 25 Card objects, each one having a unique word, a team assignment and an in-play status.
2. Stores all relevant info about the particular game (e.g. - clues given, in-play words)
3. Provides all functions required to interact with the gameboard (e.g. - selecting a card, and checking a clue would be valid)

player.py
This file contains the code to define and access player-logic:
1. Uses tools from NLTK to understand the words on the board and generate clues
2. The game allows for multiple types of players using different logics or capable of identifying different types of clues
3. Player logic is still in-progress. The public version just uses Word2Vec with the publicly available, pre-trained Google News vectors.
