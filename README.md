# Interactive Card Game

In this project, we practice object-oriented programming with MAUI, XAML and C#. The project allows the user to play a simple card game in which players win points by drawing a card with a higher rank than the house. Players can switch cards with the house before playing to improve their odds. The game continues until there are no more cards left in the card deck. 

## Exercise 1: User Interface Design with XAML
Design the user interface to implement the specification shown in the wireframe below. Debug the project and use hot reload while designing the user interface to see UI changes live as they are made.
TBD: insert wireframe
1. Analyze the wireframe to identify the necessary top-level layout and the controls necessary in this design. Compare your design with the solutions provided.
2. Create and configure the top-level layout and use XAML comments to identify significant sections of the UI design.  
3. Place controls iteratively on the page. Use one of the card-back design images for the image controls on the page.
4. Refine spacing and alignment of controls

## Exercise 2: Event Handlers
Add the event handlers required for the user interaction using the three gameplay buttons: `OnDealCards`, `OnSwitchCards`, and `OnPlayCards`

## Exercise 3: Program Structure
Follow the `Card Game - Thinking Map - Simple` UML diagram and create the user-defined types that deliver the business logic of the application
1. Classes: `CardGame`, `CardDeck`, and `Card`
2. Struct: `GameScore`
3. Enum: `CardSuit`

## Exercise 4: Field Variables and Constructors
Continue building the program structure by defining the field variables that make up each user-defined type. Use the UML diagram to identify which field variables compose which type. For each type, ensure all field variables are initialized correctly in the type's constructor.
1. CardGame field Variables and constructor
2. CardDeck field Variables and constructor
3. Card field Variables and constructor
4. CardSuit field Variables and constructor
5. GameScore field Variables and constructor
6. MainPage field Variables and constructor

## Exercise 5: Properties
Examine each user-defined type shown in the UML diagram and determine the necessary access. Define corresponding properties as required to access and/or change each field variable. Note how some properties are read-only, allowing client code to only obtain the value of a field variable without being able to change it. Reflect on how the values of those field variables might change within the program. 
1. Card Properties
2. GameScore Properties
3. CardDeck Properties
4. CardGame Properties

## Exercise 6: Methods
Business logic is implemented in methods. Examine each type and declare the necessary methods according to the `Card Game - Thinking Map - Full` UML diagram.
1. CardGame methods
2. CardDeck methods

## Exercise 7: Branching with `if` and `switch`
Practice controlling program flow with branches implemented with `if` and `switch` statements and expressions.
1. `if Statements`: Implement the `CardGame.DetermineCardRank` method to determine the rank of a card to ensure Ace has the highest rank despite having the lowest value using an if statement
2. `if Statements`: Implement the playing of a round in `CardGame.PlayRound` to determine who won the round depending on the rank of the respective cards of the player and house using an if-else-if statement.
3. Conditional Expressions. Simplify the implementation of DetermineCardRank by replacing the if statement with a conditional expression.
4. `switch` Statements. Implement the `Card.CardName` read-only property to determine the name of a card given its value (e.g. 12 is Queen)

## Exercise 8: Loops
Practice controlling the program flow with loop statements.
1. `for` Loops: Create all the cards in the deck using for loops in the `CardDeck.CreateCards` method. How many loops are needed? How are loops organized in the flow of the flow of the program?
2. `for` Loops: Shuffle the cards in the deck using a standard Fisher-Yates algorithm implemented with a `for` loop inside the CardDeck.ShuffleCards method.

## Exercise 9. 
Implement the user interaction to allow the user to play the game.
1. Deal Cards
2. Switch Cards
3. Play Cards
