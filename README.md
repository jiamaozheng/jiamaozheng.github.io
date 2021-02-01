## Assignment 2

### Requirements

3/3 | Model and Data
:---: | :---
2/2 | Custom class "Animal" that conforms to CustomStringConvertible
0.5/0.5 | Prints animal info to console via description property
0.5/0.5 | "Animals" array is shuffled when app is launched

4/4 | User Interface
:---: | :---
1/1 | UIScrollView's contentSize is 3x wider than the screen with paging enabled
1/1 | 3 UIButtons display animal names
1/1 | 3 UIImageViews display animal images
1/1 | Uses for loop with varying x coordinate to populate UIButtons and UIImageViews

4/4 | Animal Name Button
:---: | :---
1/1 | Uses button tag to identify correct animal object
1/1 | UIAlertController displays animal's name and age
2/2 | Animal sound plays

3/3 | Animal Species Label
:---: | :---
1/1 | Label does not scroll with the rest of the screen
1/1 | Label changes animal name using UIScrollViewDelegate
1/1 | Label fades in and out using the alpha property

3.5/4 | Code Quality
:---: | :---
0.75/1 | Best Practice
0.75/1 | Well-Formatted
1/1 | Clearly Written
1/1 | Concise

2/2 | Miscellaneous
:---: | :---
0.5/0.5 | Compiles with no warnings or errors
0.5/0.5 | Two GitHub branches
0.5/0.5 | Custom icon
0.5/0.5 | Cites sources

### Comments

Nice job with functionality, you've got everything working as it should.

---

Your `viewDidLoad` method in `ViewController.swift` is performing many different tasks.
This is a method where many tasks *will* be kicked off, but we should split the code for 
those tasks into single-function helper methods. Here's an example of how we could better 
encapsulate this code (and in turn make it both more readable and easier to follow):

Task 1: `func populateAnimalsArray() {}`

Task 2: `func configureButtonsAndImageViews() {}`

What code would go in each of these functions? (rhetorical question, just think about it)

Note that the names of these methods read like plain English and tell you exactly what 
they do. This indicates that a method is well-named.

---

In Swift, we `camelCase`, not `snake_case` or `SNAKE_CASE`

`let SCREEN_WIDTH: Int = 414` -> `let screenWidth: Int = 414`

---

Please delete your old commented-out code.

---

Lifecycle functions (including `viewDidLoad` should be below the class-level variables and above
other functions in the view controller.

---

Let me know if you have questions!

### Score

#### 19.5/20
