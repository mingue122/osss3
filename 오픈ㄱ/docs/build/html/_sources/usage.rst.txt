Usage Guide
===========

This guide explains the usage of the `total_game` class, including its key functions and features.

Introduction
------------
The `total_game` class provides a suite of utility functions and mini-games, such as:

- Roulette game
- Guess the person game
- Pronunciation evaluation
- Group photo analyzer
- Receipt splitting calculator

Each functionality is detailed below.

Roulette Game
-------------
The `RouletteGame` function runs a roulette game where users can spin the wheel and stop it to get a random result.

**Function Signature**:

.. code-block:: python

   def RouletteGame(values: list[str]) -> None

**Parameters**:

- `values (list[str])`: A list of strings to display on the roulette segments.

**Description**:

- Users click to spin the roulette and click again to stop it.
- The result is displayed in the console and visually below the roulette.

**Example**:

.. code-block:: python

   game = total_game()
   game.RouletteGame(["Option1", "Option2", "Option3"])

Guess the Person Game
---------------------
The `GuessPersonGame` function presents a game where users guess the name of a person based on a displayed image.

**Function Signature**:

.. code-block:: python

   def GuessPersonGame(images: list[dict]) -> None

**Parameters**:

- `images (list[dict])`: A list of dictionaries containing `image` (path) and `answer` (correct name).

**Description**:

- Users input their guesses into a text box.
- The game tracks the score and provides feedback after each guess.

**Example**:

.. code-block:: python

   images = [
       {"image": "path_to_image1.jpg", "answer": "Person1"},
       {"image": "path_to_image2.jpg", "answer": "Person2"}
   ]
   game = total_game()
   game.GuessPersonGame(images)

Pronunciation Evaluation
-------------------------
The `PronunciationApp` function evaluates a user's pronunciation by comparing spoken input with predefined sentences.

**Function Signature**:

.. code-block:: python

   def PronunciationApp() -> None

**Description**:

- Users read aloud a randomly chosen sentence.
- The program analyzes the accuracy of the pronunciation and provides feedback.

**Example**:

.. code-block:: python

   game = total_game()
   game.PronunciationApp()

Group Photo Analyzer
--------------------
The `GroupPhotoAnalyzerApp` function analyzes a group photo for specific hand gestures or poses.

**Function Signature**:

.. code-block:: python

   def GroupPhotoAnalyzerApp() -> None

**Description**:

- Users upload a group photo.
- The program detects features such as thumbs-up gestures or V poses.

**Example**:

.. code-block:: python

   game = total_game()
   game.GroupPhotoAnalyzerApp()

Receipt Splitting Calculator
----------------------------
The `Receipt` function extracts total amounts from a receipt image and calculates the per-person cost.

**Function Signature**:

.. code-block:: python

   def Receipt() -> None

**Description**:

- Users upload a receipt image and input the number of people to split the cost.
- The program extracts the total amount from the receipt and calculates the split cost.

**Example**:

.. code-block:: python

   game = total_game()
   game.Receipt()

Additional Notes
----------------
For more details on each function, refer to the inline comments in the source code or contact the development team.
