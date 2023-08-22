# Introduction

Touchegg is a Linux utility that interprets multi-touch gestures on touchpads and maps them to specific actions. By utilizing Touchegg, you can enhance your touchpad experience by assigning gestures like swipes, pinches, and taps to perform functions like window management, application switching, and more.

## Installation

To get started with Touchegg, follow these steps:

Install Touchegg: You can either download Touchegg from the official repository or install it using a package manager.

```
  sudo add-apt-repository ppa:touchegg/stable
  sudo apt update
  sudo apt install touchegg
```

Enable and Start: Enable and start the Touchegg service if it's not done automatically during installation.

```
  sudo systemctl start touchegg
  sudo systemctl enable touchegg
```

Configure Gestures: Once Touchegg is installed, you need to configure the gestures according to your preferences.

## Configuration

Touchegg configuration involves defining what actions should be triggered by specific multi-touch gestures.

``` 
git clone https://github.com/priyaranjankumar/touchegg.conf.git
cd touchegg.conf
cp touchegg.conf ~/.config/touchegg/
```

## Usage

You may need to restart your system for the changes to take effect. Once you've restarted, you can start using Touchegg to perform various actions using multi-touch gestures.

## Gestures

gesttures included im this config file are

```bash
Swipe 3 finger
 |
 |--UP:    MAXIMIZE_RESTORE_WINDOW
 |--DOWN:  MINIMIZE_WINDOW
 |--LEFT:  TILE_WINDOW
 |--RIGHT: TILE_WINDOW

Swipe 4 finger
 |
 |--UP:    SEND_KEYS Super
 |--DOWN:  SEND_KEYS Super
 |--LEFT:  CHANGE_DESKTOP
 |--RIGHT: CHANGE_DESKTOP

Pinch 2 finger (Google-chrome,Chromium-browser,firefox)
 |
 |--IN:    ZOOM IN
 |--OUT:   ZOOM OUT

Pinch 3 finger
 |
 |--IN:    CLOSE_WINDOW

Pinch 4 finger
 |
 |--IN:    SEND_KEYS Super+A
 |--OUT:   SHOW_DESKTOP

Tap 2 finger
 |
 |:        RIGHT CLICK

```

## Contributing

Contributions to Touchegg are welcome! If you'd like to contribute code, documentation, or report issues, please visit the official GitHub repository.

## License

Touchegg is released under the GNU General Public License v3.0. For more details, see the LICENSE file in the repository.
