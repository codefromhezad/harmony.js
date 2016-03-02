# Harmony.js

Harmony.js is a (small) set of helpers to work with notes, chords and finding the related audio frequencies

Warning, this is **definitely** not production ready. A lot of stuff should be reviewed or rewritten
but this is mainly for my own usage right now so ... Yeah...

This being said, this code should be considered public domain. Do whatever you want with it.




## An important note about sharp and flat notes

While sharp notes are supported in strings (like "D#") flat notes are not. At least for now.




## Documentation


##### Harmony.chordInfo(chordName)

Returns an object containing infos about a chord. Only triads are supported for now, so `chordName` is expected 
to have one of the following forms (example with C#) :

* Major : C#
* Minor : C#m
* Diminished : C#dim
* Augmented : C#aug

###### Example

```javascript
Harmony.chordInfo("C#dim")
{root: "C#", family: "triadic", type: "dim"}
```


##### Harmony.addSemitones(noteName, octave, numSemitones)

Adds `numSemitones` to `noteName`. The octave of the resulting note will be appended to the note name.

###### Example

```javascript
// Adds 6 semitones to G#4
Harmony.addSemitones("G#", 4, 6)
"D5"
```


