# Catppuccin Gnome Guide

A comprehensive guide for ricing with catppuccin theme as a base.

## Features

- Easy installation instructions
- Full customization guide
- Extensions that are useful
- GNOME customization tips


## Visual Examples

**Desktop:**
![Catppuccin Theme](./images/1.png)

**Terminal:**
![Catppuccin Theme](./images/3.png)

**Files and Brave:**
![Catppuccin Theme](./images/4.png)

**Menus:**
![Catppuccin Theme](./images/5.png)

---

## Before installing the theme

Install all necessary components so the theme works:

### Installation Commands by Distribution

| Package | Ubuntu/Debian | Arch/Manjaro | Fedora |
|---------|---------------|--------------|--------|
| **GNOME Tweaks** | `sudo apt install gnome-tweaks` | `sudo pacman -S gnome-tweaks` | `sudo dnf install gnome-tweaks` |
| **Extensions Manager** | `sudo apt install gnome-extensions-app` | `sudo pacman -S gnome-extensions-app` | `sudo dnf install gnome-extensions-app` |

### User Themes Extension

1. Open GNOME Extensions Manager
2. Search for "User Themes"
3. You can Install from: https://extensions.gnome.org/extension/19/user-themes/

### Create Required Folders

Create these folders in your home directory (if not created previously):

```bash
mkdir -p ~/.themes
mkdir -p ~/.icons
```

---

## Installation

### Installing the GTK Theme

**Theme:** https://github.com/Fausto-Korpsvart/Catppuccin-GTK-Theme

#### Steps:

1. Clone or download the repository:
```bash
git clone https://github.com/Fausto-Korpsvart/Catppuccin-GTK-Theme.git
cd Catppuccin-GTK-Theme-main/themes
```
2. Run the installation script:
```bash
./install.sh
```
3. Choose your preferred settings when prompted (Follow official GitHub guide):
- Flavor: Mocha, Macchiato, Frappe, or Latte
- Tone: Dark or Light
- Accent Color: Choose your preferred accent

4. **Important:** Add the `-l` flag to link the theme to libadwaita apps:
```bash
./install.sh -l
```

5. Apply the theme in GNOME Tweaks:
- Open GNOME Tweaks
- Go to Appearance → Themes
- Select your installed Catppuccin theme

**Note:** Sometimes you need to log out and log in to see the changes. 

### Installing Icon Pack

**Icons:** Adwaita (default) or any icon pack from https://www.gnome-look.org

#### Steps:
1. Download your preferred icon pack (Adwaita comes pre-installed)
2. Extract to the `.icons` folder
3. Apply the icons in GNOME Tweaks:
- Open GNOME Tweaks
- Go to Appearance → Icons
- Select your preferred icon theme


### Installing the Cursor Theme

**Cursor:** Any cursor from https://www.gnome-look.org

#### Steps:
1. Download your preferred cursor pack (The one I use: https://www.gnome-look.org/p/1346778)
2. Extract to the `.icons` folder
3. Apply the cursor in GNOME Tweaks:
- Open GNOME Tweaks
- Go to Appearance → Cursors
- Select your downloaded cursor theme

### Installing the fonts

**Fonts:** Any font from https://fonts.google.com/ or use the already installed ones

#### Steps:
1. Download your preferred font (The one I use: https://fonts.google.com/specimen/Comic+Neue)
2. Extract to the fonts folder:
```bash
mkdir -p ~/.local/share/fonts
unzip font-name.zip -d ~/.local/share/fonts
```
3. Refresh the font cache:
```bash
fc-cache -fv
```
4. Apply the font in GNOME Tweaks:
- Open GNOME Tweaks
- Go to fonts
- Select your downloaded font

---

## Extensions

To enhance your Catppuccin rice, you'll need extensions. You can search here: https://extensions.gnome.org/

The ones I recommend/use are listed below, but don't forget to explore and find the ones you like:

### Blur My Shell:

**Link:** https://extensions.gnome.org/extension/3193/blur-my-shell/

**Description:** It blurs many apps, menus, and the shell itself. Visually beautiful.

**Recommended Configuration:**

#### Panel Blur
- **Status:** Off

#### General View
- **Background Blur:** On
- **Flux:** Default
- **Style:** Light
- **Folder Blur:** On
- **Sigma:** 30
- **Brightness:** 0.60

#### Dialogs
- **Transparent:** On

#### Dash to Dock
- **Status:** Off

#### Apps
- **Status:** On
- **Sigma:** 10
- **Brightness:** 1
- **Opacity:** 200
- **Focused Opaque App:** On
- **General View Blur:** On
- **Activate All by Default:** On

---

### Extension List:

**Link:** https://extensions.gnome.org/extension/3088/extension-list/

**Description:** It shows a puzzle piece icon in the top bar so you can see and manage extensions without opening the Extensions Manager app.

---

### Logo Menu:

**Link:** https://extensions.gnome.org/extension/4451/logo-menu/

**Description:** It shous a logo in the top bar with many functions, as open the terminal. I actually don't use it, only for decoration haha

---

### Media Controls

**Description:** Media player controls displayed in the top bar showing what you're currently listening to. Super useful for studying or working without having to switch to the music player app.

---

### Open Bar

**Link:** https://extensions.gnome.org/extension/6580/open-bar/

**Description:** Extension for customizing open bar (The colors in the previwe images are thanks to this extension)


**Recommended Configuration:** (The options I don't put is cause i left in default)

#### Top Bar Properties
- **Type of Bar:** Floating
- **Bar Height:** 40
- **Bar Margins:** 4
- **Apply in Overview:** Off

#### Bar Foreground
- **Auto FG Color:** Off
- **FG Color:** #181927
- **FG Alpha:** 1
- **Panel Font:** Comic Neue Bold 12

#### Bar Background
- **Box/Margins Alpha:** 0
- **Bar BG Color:** #494D64
- **Bar BG Alpha:** 0,90
- **Apply Candy Bar palette:** On
- **For candy Bar Colors visit this website (I use frappe ones):** https://catppuccin.com/palette/
- **Candy BG Alpha:** 0,90
- **Panel Shadow:** Off

#### Bar Border
- **Width:** 2,0
- **Apply Width to:** ALL
- **Corner Radius:** 20
- **Apply Radius to:** ALL
- **Color:** #F4DBD6
---
