# 🎲 Dice & Flip - Terminal Fortune Tools

> Beautiful, animated coin flipping and dice rolling right in your terminal

Bring a touch of chance and excitement to your command line with smooth animations, colorful output, and instant results. Perfect for making decisions, playing tabletop games, or just having fun!

---

## ✨ Features

### 🪙 Coin Flip
- **Smooth animations** with spinning effects
- **Beautiful ASCII art** display for heads and tails
- **Multi-flip mode** with statistics tracking
- **Color-coded results** for easy reading

### 🎲 Dice Roller
- **Any-sided dice** - from d4 to d100 and beyond
- **Multiple dice** - roll as many as you need
- **Auto-totaling** for quick math
- **Special roll detection** - critical hits, fumbles, and max rolls
- **Visual dice faces** using Unicode symbols
- **D&D ready** - supports all standard RPG dice

---

## 🚀 Installation

### Quick Setup

1. **Copy the functions** to your `~/.zshrc` file:
```bash
# Simply paste the entire script at the end of your ~/.zshrc
```

2. **Reload your shell**:
```bash
source ~/.zshrc
```

3. **Start playing**:
```bash
flip
dice
```

That's it! 🎉

---

## 📖 Usage

### Coin Flip Commands

#### Single Flip
```bash
flip
```
Flips a single coin with a beautiful animation and displays either HEADS or TAILS.

#### Multiple Flips
```bash
flipx        # Flips 5 coins (default)
flipx 10     # Flips 10 coins
flipx 100    # Flips 100 coins
```
Shows each result (H/T) and provides statistics at the end.

---

### Dice Roller Commands

#### Basic Roll
```bash
dice         # Rolls a single d6 (standard die)
```

#### Multiple Dice
```bash
dice 2       # Rolls 2d6
dice 3       # Rolls 3d6
dice 5       # Rolls 5d6
```

#### Custom Sided Dice
```bash
dice 1 20    # Rolls 1d20
dice 2 10    # Rolls 2d10
dice 4 8     # Rolls 4d8
dice 3 100   # Rolls 3d100
```

**Syntax:** `dice [number of dice] [number of sides]`

---

## 🎯 Examples

### Making a Decision
```bash
$ flip
🪙  Flipping coin...
   ↻
   ↺
   ↻

╔═══════════════╗
║               ║
║     HEADS     ║
║       ◉       ║
║               ║
╚═══════════════╝
```

### Rolling for D&D
```bash
$ dice 1 20
🎲  Rolling 1d20...

╔════════════════════╗
║ Die #1: ⚅ ║
╠════════════════════╣
║ ★ CRITICAL! ★    ║
╚════════════════════╝
```

### Testing Probability
```bash
$ flipx 20
🪙  Flipping 20 coins...

H T H H T T H T H H 
T H H H T H T H H T 

╔═══════════════════╗
║ Heads: 12        ║
║ Tails: 8         ║
╚═══════════════════╝
```

---

## 🎨 Features Breakdown

| Feature | Coin Flip | Dice Roller |
|---------|-----------|-------------|
| Animations | ✅ Spinning coin | ✅ Rolling animation |
| Color Output | ✅ Green/Blue themes | ✅ Rainbow dice faces |
| Multiple Rolls | ✅ Via `flipx` | ✅ Native support |
| Statistics | ✅ Heads/Tails count | ✅ Total sum |
| Special Events | ❌ | ✅ Critical/Fumble detection |
| Custom Options | ✅ Number of flips | ✅ Dice count & sides |

---

## 🎲 Common Use Cases

- **Decision Making** - Can't decide? Let fate choose!
- **Tabletop Gaming** - D&D, Pathfinder, or any RPG
- **Probability Learning** - See randomness in action
- **Settling Arguments** - Fair and unbiased
- **Game Development** - Quick random number generation
- **Fun Breaks** - Add some excitement to your terminal sessions

---

## 💡 Pro Tips

### Quick Aliases
Add these to your `.zshrc` for even faster access:
```bash
alias d20="dice 1 20"
alias d6="dice 1 6"
alias coin="flip"
alias coins="flipx"
```

### Chain Commands
```bash
# Best of 3 coin flips
flip && flip && flip

# Roll initiative for 4 players
dice 1 20 && dice 1 20 && dice 1 20 && dice 1 20
```

### Piping for Scripting
```bash
# Use in scripts (capture output)
result=$(flip | grep -o "HEADS\|TAILS")
```

---

## 🌈 Color Palette

The tool uses a carefully chosen color scheme:
- 🟢 **Green** - Heads, high rolls, success
- 🔵 **Blue** - Tails, standard results
- 🟡 **Yellow** - Borders, attention
- 🔴 **Red** - Fumbles, low rolls
- 🟣 **Magenta** - Critical successes
- 🔷 **Cyan** - Headers, information

---

## 🛠️ Technical Details

- **Shell:** Zsh (compatible with Bash with minor modifications)
- **Dependencies:** None! Pure shell scripting
- **File Size:** ~6KB
- **Performance:** Instant results, smooth animations
- **Platform:** Works on macOS, Linux, and WSL

---

## 🤝 Contributing

🤝 Contributing

Contributions are welcome! Feel free to:

- 🐛 Report bugs
- 💡 Suggest new features
- 🔧 Submit pull requests


Ideas for future features:
- Loaded dice mode (weighted probabilities)
- Dice rolling history
- Save favorite roll configurations
- Sound effects (optional)
- Custom coin sides (not just heads/tails)

---

## 📜 License

Free to use, modify, and share. Have fun! 🎉

---

## 🎮 Happy Rolling!

Made with ❤️ for terminal enthusiasts and tabletop gamers everywhere.

*May the odds be ever in your favor!* 🍀
