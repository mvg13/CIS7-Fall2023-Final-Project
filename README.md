# Black Jack Game by WC4N
WC4N members - Pedro Sandoval, Dyson Lewis, Matthew Godinez

Published : 12/10/2023

**How to Use the Program:**

Compile the program using a C++ compiler (e.g., g++), or an IDE.
Run the executable file generated.

Follow on-screen prompts to:
Place bets: Enter the desired bet amount when prompted.
Choose actions during your turn: Enter the corresponding number for the action (e.g., 1 for Hit, 2 for Double, 3 for Stand).
Decide on split actions if applicable.

***Additional Notes***
The game loop allows for multiple rounds until the player decides to stop.
Make sure to follow the on-screen instructions for input during the game.

***2. Project Information and details:***
·   	What problems are you solving in this project? 

•	The problems that need to be solved for this project are that it must show the dealer’s hand as well as the players. 

•	It must show the winning probability for each player hand before and after card hit. 

•	Must utilize common Black Jack strategies in the program. “Soft Hand, Doubling down, and Splitting pairs.” 

•	Program must also randomize or shuffle the deck before each game. 
Project Details/Breakdown:

***Part 1: Game Initialization and Setup - completed by Dyson Lewis***

***Responsibilities:***
•	Initialize the deck of cards.
•	Implement functions to deal cards to the player and dealer.
•	Set up initial probabilities and calculations based on starting hands and bets.
•	Create structures for managing the game state (player's hand, dealer's hand, deck).

***Pseudo-code Sections:***
•	Deck initialization.
•	Dealing cards.
•	Initial probability calculations based on bets.
•	Basic game state management.

***Part 2: Player Actions and Probabilities - completed by Pedro Sandoval***

***Responsibilities:***
•	Implement player actions (hit, stand, double down, split).
•	Calculate probabilities after each action based on the updated hand.
•	Integrate decision-making logic using basic strategy tables.
•	Manage the loop for player actions until the player decides to stand or finishes the hand.

***Pseudo-code Sections:***
•	Player's turn logic.
•	Decision-making based on basic strategy.
•	Updating probabilities after each action.
•	Loop for player actions.

***Part 3: Dealer's Actions and Game Evaluation - completed by Matthew Godinez***

***Responsibilities:***
•	Implement the dealer's actions according to the fixed strategy.
•	Calculate probabilities for the dealer's hand.
•	Evaluate the game result (win, lose, push) and update probabilities accordingly.
•	Manage the game flow after the player's actions are completed.

***Pseudo-code Sections:***
•	Dealer's turn logic.
•	Updating probabilities for the dealer's actions.
•	Game result evaluation.
•	Final game flow management.

***·   What solutions are you implementing in the project?***
The implemented solutions revolve around creating a functional representation of the game.

***•	Game Logic Implementation:*** The program replicates the core logic of a blackjack game, including dealing cards, player decisions (hit, stand, double down, split), dealer actions, and game result evaluation.

***•	Basic Strategy Application:*** It incorporates a basic strategy for player decisions, adhering to optimal play based on the player's hand and the dealer's visible card.

***•	Probability Estimation:*** The program estimates the probability of certain outcomes based on the cards dealt, like the likelihood of the dealer's hand winning against the player's hand.

***•	Interactive Console Interface:*** Utilizing console inputs and outputs, the program enables players to interact by making choices during the game and providing game result feedback.

***•	Error Handling:*** Implemented error handling for input validation and edge cases to ensure the program operates smoothly even with unexpected user inputs.

***•	Modular Design:*** The program is divided into modular components, such as separate classes for cards, decks, hands, and game logic, promoting maintainability and reusability.

***•	Improvement Suggestions:*** Suggestions for enhancing the program include expanding rules, incorporating multiplayer functionalities, integrating betting strategies, and refining probability calculations.

These solutions collectively aim to create a functional and engaging representation of a blackjack game while allowing for future expansion and improvement.

***· Provide explanation of calculations and algorithm implementation.***
***•	Hand Value Calculation:***
	The program calculates the value of a player's or dealer's hand by summing the individual card values.
	Face cards (Jack, Queen, King) are considered as 10.
	Aces can be counted as either 1 or 11, with the program deciding the optimal value based on the hand's total value.

***•	Basic Strategy Implementation:***
	The program incorporates a basic strategy table that guides the player's decisions based on their hand and the dealer's visible card.
	It determines whether to hit, stand, double down, or split based on the optimal strategy, optimizing the player's chances of winning.

***•	Probability Estimation:***
	The program estimates probabilities by considering the cards dealt and the remaining cards in the deck.
	It estimates the likelihood of certain outcomes, such as the probability of the dealer's hand winning against the player's hand, based on the remaining cards.

***•	Card Distribution and Dealing:***
	The ‘Deck’ class manages the deck of cards and handles card distribution among players and the dealer.
	Cards are drawn randomly from the deck, simulating the dealing process in a casino.

***•	Dealer's Fixed Strategy:***
	The dealer follows a fixed strategy of hitting on 16 or below and standing on 17 or higher.
	This strategy is implemented to replicate the typical behavior of a dealer in a blackjack game.

***•	Looping and Decision-Making:***
	The program employs loops and conditional statements to facilitate player decisions and game flow.

	It continuously loops through player turns, dealer turns, and game evaluation until the player decides to exit the game.

***•	Error Handling and Validation:***
	The program includes error handling mechanisms to validate user inputs, ensuring proper interaction and preventing unexpected crashes due to invalid inputs.

***·What is the program objectives? Explain how your program is interacting with the user and its purpose.***
The program's objective is to represent a Black Jack casino game using a single card deck. The player is given probability odds after the initial hand is shown. Each hit the user or dealer takes will update those odds. The program interacts with the user by displaying a welcome message during the start of the program. Then it will ask the user if they want to play, learn the rules, or quit the program. After the user inputs a response the program will operate accordingly. If they want to play the program will deal the starting hands. Another message is displayed before the user that prompts them to hit or stay. The prompting of the user to input a selection is how the user and program interact with each other during the game. 

***·   How are discrete structures implemented in the C++ program?***
***•	Arrays/Lists:*** Representing the deck of cards. The player’s and dealer’s hands.

***•	Probabilities:*** Calculating and updating probabilities after each action, considering possible outcomes.

***•	Decision Points:*** Using basic strategy tables to determine player actions based on their hand and the dealer’s visible card.

***•	Loop Structures:*** Managing the game flow for player’s actions, dealer’s actions, and game evaluation.

***•	Conditional Statements:*** Implementing decision-making logic based on player’s actions and dealer’s strategy. 

***·   What are the limitations of the program?***

***•	Simplified Rules:*** The game follows a basic set of rules. It doesn't incorporate all the complexities and variations found in real casinos, such as splitting multiple times, insurance bets, or specific casino rules.

***•	Single Player vs. Dealer:*** It's designed for a single player against the dealer. Real casinos can have multiple players at the same table, leading to different strategies and interactions among players.

***•	Lack of Betting Strategy:*** The game doesn't include betting strategies like doubling bets after wins or losses, which are common in blackjack.

***•	Fixed Dealer Strategy:*** The dealer has a fixed strategy to hit below 17. Human dealers may follow different strategies based on casino rules or circumstances.

***•	Simplified Probability Estimation:*** The program estimates probabilities based on remaining cards. It doesn't consider card counting or complex mathematical strategies often employed in real blackjack games.

***·   Provide recommendations on improving the limitations of the program.***

***•	Multiplayer Functionality:*** Enhance the game to accommodate multiple players, allowing interaction between players or even introducing multiplayer modes.

***•	More Realistic Rules:*** Incorporate additional rules found in casinos, such as splitting multiple times, insurance bets, or surrender options, to make the game more authentic.

***•	Advanced Betting Strategies:*** Implement various betting strategies (like Martingale or Paroli) to make the game more engaging and strategic for players.

***•	Adaptive Dealer Strategy:*** Allow the dealer to follow different strategies based on the game's circumstances, making it more challenging for the player.

***•	 Advanced Probability Calculation:*** Implement more sophisticated probability estimation, considering factors like card counting or more advanced mathematical models for estimating odds.
	
  These enhancements can provide a more realistic and engaging blackjack gaming experience. They offer players a broader range of choices and strategies while adhering more closely to the dynamics found in actual casino blackjack games.

***3. Pseudocode:***
Version 1
—----------------------------------------------------------------------------------------------------------
// Initialize deck of cards and player’s & dealers hands
deck = initializeDeck()
playerHand = []
dealerHand = []
playerBet = 0   // Initialize player’s bet to zero
 
// Get user input for placing a bet
playerBet = getPlayerBet()
 
// Calculate initial probabilities based on the bet
initialProb = calcInInitialProb(playerHand, dealerHand)
 
// Players actions loop
while playingGame:
          	//Players turn
          	action = getPlayerAction(playerHand, dealerHand)
          	if action == “hit”:
                         	playerHand += drawCard(deck)
                         	updateProbAfterHit(playerHand, dealerHand)
          	else if action == “stand”:
                         	// Player stands, proceed to dealers turn
                         	break
          	// Continue for double down and split actions
          	else if action == “double down”:
                         	// Double the bet and draw one more card
                         	doubleBet()
                         	playerHand += drawCard(deck)
                         	// Player can’t take more actions after doubling down
                         	break
          	else if action == “split”
                         	// Check if the player has a pair
                         	if isPair(playerHand):
                                       	// split the pair into two hands
                                       	hands = splitPair(playerHand)
                                       	// Play each hand separately
                         	for each hand in hands:
                                       	// Draw one card for each hand
                                       	hand += drawCard(deck)
                                       	// Update probabilities for each hand
                                       	updateProbAfterSplit(hand, dealerHand)
                         	// Player can’t take more actions after splitting hands
                         	break
// Dealer’s turn
while dealerHand < 17;
          	dealerHand += drawCard(deck)
          	updateProbAfterDealerHit(playerHand, dealerHand)
 
// Evaluate game result and update probabilities
gameResult = evaluateGame(playerHand, dealerHand)
updateProbAfterGameResult(gameResult)
—------------------------------------------------------------------------------------------------------------------





