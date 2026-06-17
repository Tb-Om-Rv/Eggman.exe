Eggman.exe

> A "horror" game where you gotta outrun the killer with sick parkour and awesome abilities, and escape through the ring when timer reaches 80

[Optional: drop in a screenshot or GIF of your game here so readers can see what the screen looks like when it opens.]

![screenshot](assets/screenshot.png)

## Description

What is this project? Describe the interactive experience: what kind of game/experience it is, what the player is trying to do, and what makes it interesting. (2 to 4 sentences.)
A platforming survival game, where you run right and platform. You also have abilities like a boost and double jump that will assist in your escape. Jump into the ring that spawns at 80 seconds, if you can...

## How to Run

1. Make sure you have **Python 3.13** installed.
2. Install the dependencies:
   *For most of you, this is just `pip install pygame-ce`.*
3. Run the game:
   ```
   python main.py
   ```

## Controls

| Input             | Action                          |
| ----------------- | ------------------------------- |
| Arrow keys / WASD | A = move left \| D = move right |
| Spacebar          | Jump / Double jump in the air   |
| E                 | horizontal speed boost          |
| Mouse             | nothing                         |
| Esc               | nothing                         |

## Features

- [x] Screen opens to show the environment
- [x] Elements drawn on the screen  [player, killer , environment, timer, legit everything]
- [x] User-controlled elements [the player]
- [x] [opening and closing cutscene, animations]

## Dependencies

- Python 3.13
- pygame-ce
- [any other PyPI libraries - list them, or write "none beyond pygame"]
- random
## Assets

List any images, sounds, fonts, or other files in the `assets/` folder, and where each came from:

- `assets/[file]` - [made by me / source + link]
- background, terrain, ring textures- [From the sonic games from SEGA, they dont have a link cuz i just screenshotted them]
- Eggman - [pixilart, https://www.pixilart.com/art/the-eggman-sprite-sheet-sr5zb6f708650eaws3]
- 2011x - [pixilart, https://www.pixilart.com/art/2011x-sprites-sr5zc097cb9268aws3]
- Timer - [From the game Outcome Memories on Roblox, https://www.roblox.com/games/14608970270/Outcome-Memories-v0-2]
- Intro voice - [youtube, https://www.youtube.com/watch?v=miIS9FeOHL4]
- Gameplay song - [youtube, https://www.youtube.com/watch?v=PEdoXfsQ3H8&list=RDPEdoXfsQ3H8&start_radio=1]
- Intro font - [Font meme, https://fontmeme.com/fonts/sonic-roco-font/]
- Jetpack icon - [vecteezy, https://www.vecteezy.com/vector-art/14717298-jetpack-vector-icon]
- Double jump icon - [the noun project, https://thenounproject.com/browse/icons/term/effect-double-jump/]

*(If everything is your own, just say so. Credit anything you didn't make.)*

## Starting Point (Class Code)

State which code from class you used as a starting point, as required by the guardrails:

- Started from `[e.g. 10_pygame_collision.py]` - used for collision detection for player, killer, ground, environment, ring

## AI Disclosure

Disclose code or ideas where AI was used, including the **model** and **line numbers / commits**. Per the rubric, copy-and-pasted AI code is discouraged and, if used, **pasted lines need your own explanation of what it does and why**

You could use the table below or just list using bullets.

**Model(s) used:** [gemini flash extended]

| Lines / Commit            | What it does (in my own words)                                                                               | Why I used it                                                                                 | AI vs. my own                                                         |
| ------------------------- | ------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------- |
| `main.py` lines [25-35]   | creates a cache that stores all images to quickly pull from during gameplay                                  | game kept lagging in between chunks loading because it had to pull images from drive mid-game | copy-pasted                                                           |
| `main.py` lines [231]     | plays through the first two frames, but stays on the second one, does not cycle through all the frames again | didn't want jumpsquat to loop mid-air                                                         | Asked it for a function that stops at the last one                    |
| `main.py` lines [521-522] | a loop for the layouts above                                                                                 | kept getting errors when I just used the variable x for the loop                              | Asked it why it was bugging out, then I just put more variables there |
| `main.py` lines [679]     | rounds to nearest integer and makes t positive                                                               | gravity kept freaking out with decimals and sometimes negative #                              | asked it for a function that rounds and makes it positive             |

*(If no AI was used at all, write "No AI was used in this project." If AI was only used to learn concepts and no code was pasted, say that explicitly.)*

## Known Bugs / Limitations

- [terrain on the left unloads after like 3000 pixels, so if you are good enough and juke the killer you can fall through the map]

## Possible Future Improvements

- [A stun ability and maybe a title screen ]

## Author

Terrence Ho