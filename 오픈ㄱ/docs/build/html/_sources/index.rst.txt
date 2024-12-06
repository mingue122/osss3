oss24 documentation
===================

Add your content using ``reStructuredText`` syntax. See the
`reStructuredText <https://www.sphinx-doc.org/en/master/usage/restructuredtext/index.html>`_
documentation for details.


.. toctree::
   :maxdepth: 2
   :caption: Contents:

   
   usage

Key Functions
=============

Roulette Game
-------------
.. py:function:: total_game.RouletteGame(values)

   This function runs the roulette game where the user can click to spin the wheel and click again to stop it.

   **Parameters:**
   - `values (list[str])`: A list of values to display on the roulette.

   **Raises:**
   - `ValueError`: If the `values` list is empty.

   **Example:**
   .. code-block:: python

      game = total_game()
      game.RouletteGame(["Option1", "Option2", "Option3"])

Guess Person Game
-----------------
.. py:function:: total_game.GuessPersonGame(images)

   This function allows users to play a guessing game with random images and answers.

   **Parameters:**
   - `images (list[dict])`: A list of dictionaries containing image paths and answers.

   **Example:**
   .. code-block:: python

      images = [
          {"image": "person1.jpg", "answer": "Alice"},
          {"image": "person2.jpg", "answer": "Bob"}
      ]
      game.GuessPersonGame(images)

Receipt Calculation
-------------------
.. py:function:: total_game.Receipt()

   This function extracts the total amount from an image of a receipt and divides it among a given number of people.

   **Example:**
   .. code-block:: python

      game = total_game()
      game.Receipt()

