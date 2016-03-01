# Harmony.js

### A set of helpers to work with notes, chords and finding the related audio frequencies

Warning, this is *definitely* not production ready. A lot of stuff should be reviewed or rewritten
but this is mainly for my own usage right now so using it is pretty risky as-is.

This being said, do whatever you want with it.


## Helpers

### Harmony.chordInfo(chordName)

	Returns an object containing infos about a chord (only triadic chords are supported for now)

#### Example

	Harmony.chordInfo("C#dim")

	=> {root: "C#", family: "triadic", type: "dim"}