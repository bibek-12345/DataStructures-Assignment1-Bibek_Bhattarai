Name: Bibek Bhattarai
ID: C0913757
Instructions on how to run your code
Install JDK: Ensure you have the Java Development Kit (JDK) installed. You can download it from the Oracle website.

Create Java File:

Open your IDE or text editor.
Create a file named name.java.
Copy the Code: Paste the name class code into name.java.

Compile the Code:

Open a terminal or command prompt.
Navigate to the directory with the file.
Run: javac name.java
After successful compilation, execute:
java name

1. **The Array Artifact **
   Implement a class `ArtifactVault` that uses an array to store ancient artifacts. Include methods to:
   - Add an artifact to the first empty slot
   - Remove an artifact by its name
   - Find an artifact using linear search
   - Find an artifact using binary search (assume the array is kept sorted by artifact age)


# A brief description of above challenge and how I approached it
The challenge was to develop a class called ArtifactVault that effectively manages a collection of artifacts, enabling operations such as adding, removing, and searching for items while displaying the collection. My approach involved using a fixed-size array to store artifact names, which allowed for efficient memory usage and quick access. In the addArtifact method, I ensured that the array remains sorted by sorting it immediately after each addition, which facilitates efficient searching. For artifact removal, the removeArtifact method finds the specified artifact and shifts the remaining elements to fill the gap, thus maintaining the integrity of the array. To support searching, I implemented both linear and binary search methods, allowing for quick location of artifacts based on their names. Overall, this design provides a structured and efficient way to manage a collection of artifacts within the vault.

2. **The Linked List Labyrinth (20 points)**
   Create a `LabyrinthPath` class using a singly linked list. Implement methods to:
   - Add a new location to the path
   - Remove the last visited location
   - Check if the path contains a loop (trap)
   - Print the entire path
# A brief description of above challenge and how I approached it
The challenge involved creating a LabyrinthPath class using a singly linked list to manage locations in a labyrinth. The key functionalities included:
1.	Data Structure: Used a linked list where each Node represents a location.
2.	Adding Locations: Implemented addLocation to add nodes to the end of the list.
3.	Removing Locations: Created removeLastLocation to remove the last node in the list.
4.	Loop Detection: Used Floyd’s Cycle Detection algorithm in the containsLoop method to check for cycles.
5.	Path Printing: Developed printPath to display all locations in the list.
The main method tests the functionalities by adding, removing, and printing locations. This structure provides dynamic management of the labyrinth path with efficient operations.

3. **The Stack of Ancient Texts (20 points)**
   Develop a `ScrollStack` class that uses a stack to manage ancient scrolls. Include operations to:
   - Push a new scroll onto the stack
   - Pop the top scroll off the stack
   - Peek at the top scroll without removing it
   - Check if a specific scroll title exists in the stack
# A brief description of above challenge and how I approached it
README.MD	
The challenge involved creating a ScrollStack class that simulates a stack data structure specifically for managing scrolls represented as strings. To approach this, I designed the class with a private Stack<String> to encapsulate the stack's behavior. I implemented core methods such as pushScroll(String scroll) for adding scrolls, popScroll() for removing the top scroll (initially returning null when the stack was empty), and peekScroll() for viewing the top scroll without removal. Additionally, I included a method containsScroll(String title) to check for the existence of a specific scroll. To ensure functionality, I wrote a main method for testing the class, showcasing operations while printing the current stack state. I later enhanced the class by adding a printStack() method for easy visualization and improved error handling by throwing exceptions for empty stack scenarios instead of returning null. This structured approach ensured that the ScrollStack class was functional, maintainable, and aligned with traditional stack behavior.

4. **The Queue of Explorers (20 points)**
   Implement a `ExplorerQueue` class using a circular queue. The queue should:
   - Enqueue new explorers
   - Dequeue explorers when they enter the temple
   - Display the next explorer in line
   - Check if the queue is full or empty

# A brief description of above challenge and how i approached it
Implementing the ExplorerQueue class presented several challenges, primarily related to managing the circular behavior of the queue with an array, ensuring the capacity limits were adhered to, and handling operations on an empty queue. To address these issues, I utilized modulo operations to correctly update the front and rear indices, ensuring they wrap around the array when needed. I maintained a size counter to track the number of elements and implemented checks for full and empty conditions to manage enqueue and dequeue operations appropriately. Additionally, I focused on testing the queue's functionality by creating various scenarios in the main method, ensuring it handled edge cases effectively, such as overflow and underflow situations.

5. **The Binary Tree of Clues (20 points)**
   Create a `ClueTree` class representing a binary tree of clues. Implement methods to:
   - Insert a new clue
   - Perform in-order, pre-order, and post-order traversals
   - Find a specific clue in the tree
   - Count the total number of clues in the tree

# A brief description of above challenge and how i approached it
The challenge involved creating a binary search tree (BST) to efficiently manage and organize clues, allowing for insertion, traversal, and search functionalities. To address this, I designed a TreeNode class to represent each node in the tree, encapsulating the clue and pointers to its left and right children. This structure enables the organization of data according to BST properties, where the left child is less than the parent and the right child is greater. I implemented an insertClue method to initiate the insertion process, utilizing a recursive helper method, insertRec, to determine the appropriate position for new clues based on their comparison with existing nodes. For traversal, I provided an inOrderTraversal method, which employs another recursive method, inOrderRec, to print the clues in sorted order. Additionally, I included a findClue method to search for specific clues, enhancing the tree's utility for efficient retrieval and organized data representation.
