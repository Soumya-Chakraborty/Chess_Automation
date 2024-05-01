# chess-auto-bot
A bot for chess.com and lichess.org that automatically plays chess for you  

Chess.com  
![](match_chesscom.gif)  

Lichess.org  
![](match_lichess.gif)  
Note that the mouse is being moved by python

## How to install
1) Clone the repository or just download the repository as a .zip
2) Download Stockfish from https://stockfishchess.org/  
   **Note** that on Linux systems you must manually add execute permissions to the stockfish executable
3) Open a Terminal
4) `cd Chess-Automation`
5) Windows: `python -m venv venv`  
   Linux: `python3 -m venv venv`
6) Windows: `venv\Scripts\pip.exe install -r requirements.txt`  
   Linux: `venv/bin/pip3 install -r requirements.txt`

## How to use
1) Open a Terminal
2) `cd chess-auto-bot`
3) Windows: `venv\Scripts\python.exe src\gui.py`  
   Linux: `venv/bin/python3 src/gui.py`
4) Click Select Stockfish on the GUI that opens. This will open a file explorer. Navigate to the folder where you downloaded Stockfish and select the Stockfish executable.
5) Click Open Browser. This will open ChromeDriver and load the selected chess website.
6) Navigate to a live match (online or vs bot)
7) Click Start (or press 1)
8) Enjoy  

**Note** You can stop the bot at any time by pressing Stop or pressing 2.

## Currently supports
- Windows/Linux platforms
- Chess.com
- Lichess.org
- Playing vs humans
- Playing vs bots
- Puzzles (with option for non-stop solving):
    - [ ] chess.com
    - [x] lichess.org
- Manual mode (Press or hold 3 to move when enabled)  
  An arrow with the best move is also displayed
- Mouseless mode (The moves are made without the mouse moving, also works while the browser is at the background):
    - [ ] chess.com
    - [x] lichess.org
- Bongcloud mode ( ͡° ͜ʖ ͡° )
- Skill level selection (0-20)
- Depth level selection (1-20)
- Memory (RAM) usage selection
- CPU threads number selection
- Slow Mover option (defaults to 100, 10 &le; Slow Mover &le; 1000)  
  lower values will make Stockfish take less time in games, higher values will make it think longer
- Exporting finished games to PGN

## Disclaimer
Under no circumstances should you use this bot to cheat in online games or tournaments. This bot was made for educational purposes only.
Using this bot to cheat in online games or tournaments is against the rules of chess.com and will result in a ban.
