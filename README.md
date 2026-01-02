# MaGogmazios Reroll Planner

A comprehensive reroll planning tool for Monster Hunter Wilds Gogmazios weapon variants, featuring skill and reinforcement tracking.

## 🎮 Features

-   **Multi-weapon Support**: Track variants for all 14 weapon types (Great Sword, Long Sword, Sword & Shield, etc.)
-   **Smart Roll Management**:
    -   `+` buttons: Simulate rerolls without saving (plan ahead)
    -   `-` buttons: Commit rerolls and advance the shared seed counter
-   **Material Calculator**: Automatically calculates required materials and Oricalcite
-   **Recommendation System**: Suggests optimal reroll order based on remaining needs
-   **Dark/Light Theme**: System-adaptive theme switcher with manual override
-   **Data Persistence**: Automatic save/load via localStorage
-   **Import/Export**: Backup and restore your planning data

## 📖 How to Use

### Adding Variants

1. Click the **"+ Add variant"** button under any weapon
2. Configure:
    - Element (Fire, Water, Thunder, etc.)
    - Artian type
    - Desired skills and reinforcements
    - Target roll counts

### Roll Management

Each variant has four buttons:

-   **S+** (🔄): Plan a skill reroll (increment target only)
-   **S-** (🔄): Commit a skill reroll (decrements ALL variants)
-   **R+** (💾): Plan a reinforcement reroll (increment target only)
-   **R-** (💾): Commit a reinforcement reroll (decrements ALL variants)

### Understanding Shared Rolls

The `-` buttons affect **all weapons** because rerolls in-game share a common seed. When you save-scum a reroll:

1. Click the appropriate `-` button on the weapon you rerolled
2. This decrements the counter for ALL tracked variants
3. Plan ahead using `+` buttons to see how many rerolls you need

### Recommendations

The **"Next recommended"** section shows which variant to prioritize based on:

-   Lowest remaining skill rolls needed
-   Lowest remaining reinforcement rolls needed
-   Only shows variants that still need work

Toggle **"Show only tracked"** to hide variants with no targets set.

## 💾 Data Management

### Export

Click **Export** to download a JSON backup of your planning data.

### Import

Click **Import** and select a previously exported JSON file to restore your data.

### Reset

Click **Reset** to clear all data and start fresh (confirmation required).

## 🎨 Theme Options

Three theme modes available:

-   **💻 System**: Follows your OS preference
-   **☀️ Light**: Force light theme
-   **🌙 Dark**: Force dark theme

## 🛠️ Technical Details

-   **Single-file app**: Everything in one HTML file for easy deployment
-   **No dependencies**: Pure vanilla JavaScript + Tailwind CSS CDN
-   **Offline-capable**: Works without internet after first load
-   **Responsive**: Mobile-friendly design

## 📄 License

This work is licensed under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License](http://creativecommons.org/licenses/by-nc-nd/4.0/).

## 🙏 Credits

-   Weapon icons: Embedded base64 images
-   Monster type skills: Comprehensive list from game data

## 🐛 Known Issues

None currently. Please report issues on GitHub!

## 📝 Changelog

### v4 (Current)

-   Redesigned roll management UI with icons and help text
-   Implemented shared counter logic for committed rerolls
-   Added icon-based theme switcher
-   Fixed dark mode toggle
-   Removed global roll counters
-   Added Creative Commons license

---

Made with ❤️ for the Monster Hunter community
