# Tic-Tac-Tie 2.0
## Now written in 6502 Assembly! :)

Yeah, it's another Tic-Tac-Toe game.  Dumbest game on the planet (Rock-Paper-Scissors is more fun).  But it's still worth open-sourcing because I'm using it to practice Assembly programming.  I'm sure I'm not the first person to wish there were more simple examples out there - and mine's about as simple as a game can get while still being an actual playable game. :)

## A few technical notes

* I'm targeting the Commodore PET 2001 (which cc65 doesn't support).  I'm going with the minimal specs (BASIC v2, 8K ram etc.) and using this awesome emulator to test it: https://www.masswerk.at/pet/
* I'm using DASM as my assembler, and no crazy macros.  This is because (1) 6502 macros are inconsistent from one assembler to the next (so anyone who wants to mess with my code would have to use DASM if I did that), and (2) I haven't learned any yet.  Maybe for my first *serious* game. :)
* Currently, you have to type the BASIC command "sys 4096" to run the game.

## To-Do's

* Create my X and O graphics
* Add a loop that polls the keyboard for keys 1-9 and puts an X (or O) in the right place
* Create the "AI"
* Set up the turn system so the game is actually playable
* If possible, add a menu screen (1 vs. 2 players, choose X vs O etc.).
* Copy over pet.s from my library, so others have access to SCREEN_RAM_START, KEYBOARD and my other constants
