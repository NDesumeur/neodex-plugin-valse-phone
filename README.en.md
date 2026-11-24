# Waltz

A one-key rhythm game in the night sky: the sun and the moon spin around each other on a path of tiles. When the spinning one touches the next tile, tap: it lands, and the other one starts spinning. The path is drawn by the music. Play the 1200 tracks from the Rythme plugin, or your own music.

*Version française : [README.md](README.md)*

## Phone version

You play with one finger: tap the screen right when the orb reaches the golden tile. Tapping the game starts the song in full screen; during the game, the PAUSE button sits at the top right of the game (it stays there in full screen), and the phone's back button pauses too. After a fall, a tap resumes from the flag and the START button goes back to the beginning. The game pauses by itself when you leave the app. The offset adjusts itself after each game, which helps since a phone's sound sometimes comes a little late.

## How to play

- **Any key** (letters, arrows, Enter) or a **click**: land the orb on the golden tile, right when it touches it.
- **Reading the path**: the orb spins half a turn per beat. A **straight line** lasts one beat, a **right angle** half a beat, a **sharp turn** a quarter of a beat.
- **Three blue dots** on a tile: the orb spins slower there (a long pause in the music).
- **A pink loop**: the orb changes its spinning direction.
- **Too early or too late and you lose**: only the next tile counts, and an extra press in the beat before it loses the run. Tapping at random doesn't work. Two keys pressed almost together (under 60 ms) only count once.
- **Flags**: every 32 tiles. After a lost run, **Space** restarts from the last flag passed (no record), **R** starts again from the beginning.
- The camera follows the orb and the sky stays still: nothing gets in the way of reading the path.
- **Space**: play · **P**: pause · **Full screen** during the game.

## Accuracy and points

Notes are judged by how far they are from the right moment: **Perfect** (about ±45 ms), **Good** (±90 ms), **OK** (±140 ms), otherwise a miss.

A note's points rise by 1 % per note of combo, up to double at 100 notes in a row; a miss resets the combo. At the end, accuracy gives a grade: **S** from 95 %, **A** at 90 %, **B** at 80 %, **C** at 70 %, **D** below.

## Songs and difficulty

The **Songs** tab has the 1200 Rythme tracks, in four difficulties (Easy, Normal, Hard, Expert). Each level's difficulty is computed from its notes (density, busy passages), from 1 to 10 stars.

## My music

In **My music**, create a level from an imported **audio file** or a track from your **NeoMusic** library: the game finds its tempo and strong beats and turns them into a level, at the chosen **difficulty** (1 to 10 stars).

## Practice and figure

- **Start** (practice): begin at 25, 50 or 75 % of the song to work on a passage. Earlier notes don't count, and nothing is kept as a record.
- **Progress**: when you lose, the screen gives the share of the song you reached, and your record on this level.
- The end screen also shows **the figure drawn by the whole path**, cleared tiles in green and missed ones in red.

## Settings

- Music **volume**.
- **Hit sound**: the sound played on each note you hit, one of 10 (Soft, Clap, Wood, Kick, Crystal, Pop, Hi-hat, Snare, Pluck, Tock) or none. Losing a combo of 10 or more plays a « combo break » sound.
- **Offset** (−300 to +300 ms): it adjusts itself after each game based on your average lateness or earliness; you can also change it by hand.

## Data and sync

Your scores and grades per level and your settings are stored by NeoDex, backed up and synced between your PCs when sync is on.

## Install

In NeoDex: **NeoStore → Discover → Waltz → Install**.

Building a plugin: see the [NeoDex SDK](https://github.com/NDesumeur/neodex-sdk).

## What's new in version 2.0.0

- The game is rebuilt around strict judging: too early or too late and the run is lost (before, you could tap at random and still finish).
- Checkpoint flags every 32 tiles.
- No more camera effects (zooms, rotations) or scrolling sky: only the path moves.

## What's new in version 1.1.0

- **Gamepad**: the D-pad, A, B, X, Y and the shoulder buttons place the star; Start starts the song (A too, outside a game); Select pauses.
- **Accuracy curve** on the end screen: your precision all along the song, with missed notes marked in red underneath, to see where you lost the beat.
