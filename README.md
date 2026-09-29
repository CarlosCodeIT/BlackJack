#Linear Search Preview
1. Where does the search begin?
   * A linear search always begins at the beginning of the ArrayList. It checks the first card,
   * then the second, and continues forward one item at a time.
2. What is being compared during each pass through the loop?
   * During each pass, the algorithm compares the card's name (card.getCardName()) with the search term (searchName).
   * Only the cardName field of the Card object is used in the comparison.
3. What does break do when a matching card is found? What would happen if the break were removed?
   * break immediately stops the loop as soon as a match is found.
   * If the break were removed, the loop would continue checking every remaining card even though the desired card was already found.
   * This wastes time and could overwrite foundCard if another matching card appears later.
4. If the card you are searching for is the first card in a 52-card ArrayList, how many cards are checked?
   * Only one card needs to be checked.
6. If the card you are searching for is the last card in a 52-card ArrayList, how many cards might need to be checked?
   * Only one card needs to be checked.
5. If the card you are searching for is the last card in a 52-card ArrayList, how many cards might need to be checked?
   * All 52 cards might need to be checked before the match is found.
6. If the card you are searching for is not in the ArrayList at all, how many cards would the linear search need to check?
   * It would check all 52 cards and then conclude that the card is not present.
7. Why is this type of search called a linear search?
   * It is called a linear search because it moves through the collection in a straight line, one item after another,
   * without skipping or jumping ahead.
8. Describe a linear search algorithm in your own words.
   * A linear search looks through a list by starting at the first item and checking each one in order. You keep moving forward until
   * you either find what you're looking for or reach the end of the list. It's a simple, step by step way to search when the data isn't
   * organized in any special way.
#Short Reflection
-One thing I learned during this assignment is how important the equals() method is when storing objects in an ArrayList.
At first, I assumed java would automatically know when two Card objects were "the same," but I realized that without overriding equals(),
Java only compares memory locations, not the actual card data. Once I implemented equals() correctly, the pair checking logic started
working the way I expected. This helped me understand the difference between an object's data (like suit, name, and value) and its behavior
(the methods that operate on that data).
