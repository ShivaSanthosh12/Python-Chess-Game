# 🏆 Python Chess Game

A fully functional chess game built with Pygame, featuring a clean interface, piece movement validation, and turn-based gameplay.

## 🎮 Features

- **Complete Chess Gameplay**: All standard chess pieces with proper movement rules
- **Turn-based System**: Alternating white and black player turns
- **Move Validation**: Legal move checking for all pieces
- **Visual Feedback**: 
  - Highlighted selected pieces
  - Valid move indicators
  - Check detection with flashing king
- **Capture System**: Captured pieces displayed on the side panel
- **Game Over Detection**: Automatic winner declaration when king is captured
- **Restart Functionality**: Press ENTER to start a new game
- **Forfeit Option**: Players can forfeit their turn


## 🚀 Getting Started

### Prerequisites

- Python 3.7 or higher
- Pygame library

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/python-chess-game.git
   cd python-chess-game
   ```

2. **Install required dependencies**
   ```bash
   pip install pygame
   ```

3. **Run the game**
   ```bash
   python chess_game.py
   ```

## 📁 Project Structure

```
python-chess-game/
│
├── chess_game.py          # Main game file
├── images/                # Chess piece images
│   ├── bB.png            # Black Bishop
│   ├── bK.png            # Black King
│   ├── bN.png            # Black Knight
│   ├── bp.png            # Black Pawn
│   ├── bQ.png            # Black Queen
│   ├── bR.png            # Black Rook
│   ├── wB.png            # White Bishop
│   ├── wK.png            # White King
│   ├── wN.png            # White Knight
│   ├── wp.png            # White Pawn
│   ├── wQ.png            # White Queen
│   └── wR.png            # White Rook
├── screenshots/           # Game screenshots
├── README.md             # Project documentation
├── requirements.txt      # Python dependencies
└── LICENSE               # License file
```

## 🎯 How to Play

1. **Starting**: White pieces move first
2. **Selecting Pieces**: Click on a piece to select it (highlighted in red for white, blue for black)
3. **Moving**: Click on a valid destination square (marked with colored dots)
4. **Capturing**: Move to an opponent's square to capture their piece
5. **Check**: King will flash when in check
6. **Winning**: Capture the opponent's king to win
7. **Forfeit**: Click the "FORFEIT" button to surrender
8. **Restart**: Press ENTER after game over to start a new game

## 🔧 Game Controls

- **Mouse Click**: Select pieces and make moves
- **ENTER**: Restart game after game over
- **X Button**: Close the game

## 📋 Chess Rules Implemented

- ✅ **Pawn**: Forward movement, diagonal capture, double move from starting position
- ✅ **Rook**: Horizontal and vertical movement
- ✅ **Knight**: L-shaped movement pattern
- ✅ **Bishop**: Diagonal movement
- ✅ **Queen**: Combined rook and bishop movement
- ✅ **King**: One square in any direction
- ✅ **Piece Blocking**: Pieces cannot jump over others (except knight)
- ✅ **Capture Rules**: Cannot capture own pieces

## 🛠️ Technical Details

### Built With
- **Python 3.x**
- **Pygame** - Game development library

### Key Components
- `draw_board()` - Renders the chess board and UI
- `draw_pieces()` - Displays pieces on the board
- `check_options()` - Validates all possible moves
- `check_[piece]()` - Individual piece movement logic
- `draw_valid()` - Shows valid moves for selected piece
- `draw_check()` - Highlights king when in check


## 🐛 Known Issues

- Castling is not implemented
- En passant capture is not available
- Pawn promotion is not implemented
- Checkmate detection could be improved
