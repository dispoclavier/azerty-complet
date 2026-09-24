# Replacerulesets

Settings for the "bhughes339.replacerules" extension for VSCode.

These replacerules are intended to be added in settings.json.

## Symmetrization of chained dead keys

Chained dead keys may be symmetrized using the "bhughes339.replacerules"
extension for VSCode with a replaceruleset based on the observation that
at this point, chaining does not encompass more than four dead key strokes
other than group selection, that always trails and is thus not symmetrized.
The JSONsymmetrizeChainedDeadKeys" goes into user settings and has the "@"
prefix for subsequent multikey equivalent generation built in, for a number
of likely use cases.

## Conflictlessness check

Conflicts and duplicates can be checked following a protocol like this one,
where the first steps may be automated using the "bhughes339.replacerules"
extension for VSCode with the "prepareXComposeForCheck" replaceruleset.

 2  Case sensitive sorting, using "Tyriar.sort-lines" > F9.

 3  Checking for conflicts and duplicates:
 ^([^\s]+)\s.+\n\1(<|\s)

Sortability and readability may then be further improved using the
follow-up replaceruleset "improveXComposeSortability", where dead
keysyms missing from keysymdef.h replace the generic private use keysyms,
all dead keysyms are prefixed with an exclam so as to be sorted before
letters and digits, as well as before ASCII symbols prefixed with a percent
sign, some more letters get intuitive keysyms, and ordinary space and U200B
as well as nobreakspace and U202F are grouped conveniently and sorted last
by the means of a prepended asciitilde.

The removal of padding spaces is included, as it does not affect sorting.
This facilitates reviews for redundancies to be redacted for a streamlined
user experience.
