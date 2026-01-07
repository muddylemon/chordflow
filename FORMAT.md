# ChordFlow Format Reference

ChordFlow uses a simple text-based format to create beautiful chord sheets. This document explains the syntax and features.

## Basic Syntax

### Chords

Place chords in **square brackets** `[X]` directly before the syllable or word where the chord should be played.

```
[G]You weren't your mama's only boy
But her fav[D]orite one [G]it seems
```

**Renders as:**
```
G                   D          G
You weren't your mama's only boy
      D          G
But her favorite one it seems
```

The text following each chord will be colored to match the chord, making it easy to see which words go with which chords.

### Sections

Use **curly braces** `{Section Name}` on their own line to mark song sections like verses, choruses, bridges, etc.

```
{Verse 1}
[D]Living on the road my friend
[A]Was gonna keep you free and clean

{Chorus}
[G]All the federales say
They [D]could have had him [G]any day
```

Sections serve two purposes:
1. They appear as subtle labels in the output
2. In **Page Mode**, each section becomes its own "page" for hands-free navigation

### Instrumental Breaks

For chord-only passages (intros, outros, turnarounds), simply write chords without any lyrics:

```
{Intro}
[D] [A] [G] [D]

{Turnaround}
[D4] [D] [D4]
```

### Notes Field

Use the **Notes** field in the editor for tuning information, capo position, tempo, or any other helpful details:

```
Capo 2nd fret · Tuning: Drop D · 120 BPM
```

These appear below the song title in the display view.

---

## Display Features

### Page Mode

Click the **Pages** button to enter presentation mode. This is ideal for playing live—each section becomes its own page that fills the screen.

**Navigation:**
- Tap/click anywhere on the screen
- Press `Space` or `→` for next page
- Press `←` for previous page

### Chord Diagrams

Click the **Chords** button to show fingering diagrams for all chords in the song. Diagrams are color-coded to match the chord legend.

### Keyboard Shortcuts

| Shortcut | Action |
|----------|--------|
| `Ctrl + Enter` | Display chord sheet |
| `Escape` | Return to editor |
| `Space` / `→` | Next page (in Page Mode) |
| `←` | Previous page (in Page Mode) |

---

## Supported Chords

ChordFlow includes diagrams for these common guitar chords:

**Major:** A, B, C, D, E, F, G  
**Minor:** Am, Bm, Cm, Dm, Em, Fm, Gm  
**Seventh:** A7, B7, C7, D7, E7, F7, G7  
**Minor 7th:** Am7, Em7  
**Major 7th:** Amaj7, Cmaj7, Dmaj7, Emaj7, Fmaj7, Gmaj7  
**Sus4:** A4/Asus4, D4/Dsus4, E4/Esus4, G4/Gsus4  
**Sus2:** Asus2/A2, Dsus2/D2, Gsus2/G2  
**Add chords:** Cadd9, Dadd4, Gadd4  
**Slash chords:** G/B

Chords not in the library will still appear in the legend with colors—they just won't have diagrams.

---

## Example Song

```
{Intro}
[D] [A] [G] [D]

{Verse 1}
[D]Living on the road my friend
[A]Was gonna keep you free and clean
[G]Now you wear your skin like iron
Your [D]breath's as [A]hard as kerosene

{Chorus}
[G]All the federales say
They [D]could have had him [G]any day
[Bm]They only let him [G]hang a[A]round
Out [G]of kindness I [Bm]suppose
```

---

## Tips

1. **Mid-word chord changes:** Place the chord directly before the syllable: `fav[D]orite`

2. **Multiple chords, no lyrics:** Separate with spaces: `[D] [G] [A]`

3. **Blank lines:** Use empty lines to add visual spacing between phrases

4. **Printing:** Use your browser's print function (`Ctrl/Cmd + P`) for a clean printout

5. **Column layout:** On wider screens, lyrics automatically flow into multiple columns to maximize space
