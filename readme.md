# Speedboard

## User Story

As a new student I have trouble finding exotic characters on my keyboard, so I'd like a fun game that trains my typing skills.

## Game Play

The player hears the names of special characters as spoken words. Her objective is to find the associated key and press it. Over time, the game will focus on the keys that the player has the most trouble identifying or finding.

### Optional hint system
If the player hits the wrong key, or no key at all for a number of seconds, we display the correct symbol (in case she has trouble indentifying the key from its name)

#### Increased difficulty
The player is told to enter a sequence of characters. (for example: "shebang", "fat arrow").

#### Levels
When the player hits the correct key within a certain time window, we give positive feedback. The time window gets smaller which each level.

## Task Breakdown

- record sounds for all special characters
    - depending on context, there are multiple names for one specific character (example: 'less than'/'open angle bracket'), so we need multiple sound files for one character.
    - filenames begin with ASCII codes coded as two-digit hex numbers, followed by the character's name.
        - *Example* `7e-tilde.wav` says "tilde"
- [x]  play back a sound
- [ ] recognize a keystroke
- [ ] display some kind of feedback for each keystroke
- [ ] measure time between audio playback and keystroke
- [ ]some kind of reward
    - especially when a problematic key turns into an unproblematic key
- [ ] keep stats about timing and failure rate per audio file
- [ ] identify problematic audio files or keys
- [ ] persist the state of the game

