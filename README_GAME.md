# Snake AI Game - Instructions and Setup Guide

## Overview

Welcome to **1snakeai** - an AI-powered Snake game project! This guide will help you set up and play the game.

## Game Instructions

### Objective
Guide the snake to eat food and grow longer while avoiding:
- Collisions with the game walls
- Collisions with the snake's own body

### Controls
- **Arrow Keys** or **WASD**: Control snake direction
  - Up/W: Move upward
  - Down/S: Move downward
  - Left/A: Move left
  - Right/D: Move right

### Gameplay Rules
1. The snake starts with a small initial length
2. Food appears randomly on the game board
3. Eating food increases your score and snake length
4. The game ends when the snake hits a wall or itself
5. Higher scores are achieved by eating more food without colliding

### Scoring
- Each food eaten: +10 points
- Bonus points may be awarded for consecutive food consumption without pause

## Setup Guide

### Prerequisites
- Python 3.7 or higher
- pip (Python package manager)
- Git (for cloning the repository)

### Installation Steps

1. **Clone the Repository**
   ```bash
   git clone https://github.com/kriskoradichev-wq/1snakeai.git
   cd 1snakeai
   ```

2. **Create a Virtual Environment** (Recommended)
   ```bash
   # Windows
   python -m venv venv
   venv\Scripts\activate

   # macOS/Linux
   python3 -m venv venv
   source venv/bin/activate
   ```

3. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
   ```
   
   If `requirements.txt` doesn't exist, common dependencies may include:
   ```bash
   pip install pygame numpy
   ```

4. **Run the Game**
   ```bash
   python main.py
   ```
   
   Or if using a specific game script:
   ```bash
   python snake_game.py
   ```

### Project Structure
```
1snakeai/
├─��� README_GAME.md          # This file
├── main.py                 # Main game entry point
├── snake_game.py           # Core game logic
├── ai/                     # AI agent implementations
├── assets/                 # Game assets (sprites, sounds)
├── requirements.txt        # Python dependencies
└── README.md              # Original project README
```

## AI Features

This project includes AI capabilities for the Snake game:
- **Machine Learning Integration**: Train AI agents to play the game
- **Neural Network Support**: Deep Q-Network (DQN) or similar algorithms
- **Training Mode**: Run the game in headless mode for faster AI training
- **Visualization**: Watch your trained AI play the game

### Training the AI

```bash
# Train AI agent
python train_ai.py

# Play with trained model
python play_with_model.py --model trained_model.h5
```

## Troubleshooting

### Common Issues

**Issue**: `ModuleNotFoundError: No module named 'pygame'`
- **Solution**: Run `pip install pygame`

**Issue**: Game window won't open
- **Solution**: Ensure you have a display (for headless systems, use `--headless` flag if available)

**Issue**: Game runs slowly
- **Solution**: Reduce graphics quality or close other applications

## Development

### Running Tests
```bash
pytest tests/
```

### Code Style
Follow PEP 8 guidelines. Use `black` or `autopep8` for formatting:
```bash
pip install black
black .
```

## Contributing

Contributions are welcome! Please:
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -m 'Add feature'`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Open a Pull Request

## License

Check the LICENSE file in the repository for license information.

## Support

For issues, questions, or suggestions:
- Open an issue on GitHub
- Check existing documentation in the repository
- Review the main README.md for additional context

## Version History

- **v1.0.0** - Initial game release with basic Snake gameplay
- Future versions may include enhanced AI, graphics improvements, and multiplayer support

---

**Happy Gaming and Good Luck Training Your AI!** 🐍🤖
