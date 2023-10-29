# Wordle Buddy

Summary   | Current Release
----------|-----------------------
Version   | 2.0
Date      | September 9, 2022
Platforms | macOS, Linux (Ubuntu+), Windows
Author    | Brom Bresenham

# About
Wordle Buddy is a console-based app that assists in solving [Wordle](https://powerlanguage.co.uk/wordle/) puzzles.

# Demo
![Demo](Media/Videos/WordleBuddy.gif)

# Installation

## New Installation

1. Install [morlock.sh](https://morlock.sh)
2. `morlock install brombres/wordlebuddy`

## Updating Existing Installation
    morlock update wordlebuddy

# Usage

    USAGE
      wordlebuddy solver
      wordlebuddy game
      wordlebuddy game solver
      wordlebuddy list <pattern>
      wordlebuddy list "<pattern>" containing <letters>

    DESCRIPTION
      wordlebuddy solver
        Interactively assists in solving an online Wordle puzzle.

      wordlebuddy game
        Plays a Wordle game without solver assistance.

      wordlebuddy game solver
        Plays a Wordle game with solver assistance.

      wordlebuddy list <pattern>
        List possible words that match the given 5-character pattern.

        <pattern>
          * - Match words with any character at this position.
          A - Match words with an 'A' at this position.
          a - Match words with an 'A' NOT at this position.

        wordlebuddy list "<pattern>" containing <letters>
          Lists words matching the pattern (which can be "*****") AND
          containing all the given letters.

      EXAMPLES
        wordlebuddy list "r*O*T"
          # List words that have 'O' in the middle, end in 'T', and
          # contain an 'R' but don't start with it.

        wordlebuddy list "*O**c" containing tu
          # List words that have O as the second letter, contain 'C'
          # but not as the last letter, and contain the letters 'T'
          # and 'U' anywhere.

# Thanks
- [Wordle](https://powerlanguage.co.uk/wordle/) for a fun game.
- [Graham Allen](https://twitch.tv/graham) for introducing me to Wordle and inspiring me with his solver research:
    - [Wordle Solver Exploration Part 1](https://observablehq.com/@iamgrahamallen/wordle-solver-exploration)
    - [Wordle Solver Exploration Part 2](https://observablehq.com/@iamgrahamallen/wordle-solver-exploration-part-2)

