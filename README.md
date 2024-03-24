# tchackpoum-sfz

This is a virtual drum kit in SFZ format using samples recorded by Vincent
"[Tchackpoum](http://tchackpoum.fr/)" Sermone. The MIDI mappings are set up
with the intention of working for many popular e-drumkits (Alesis, Roland,
Simmons, et. al.) without having to futz about with MIDI note numbers.

The sound files include a combination of mono and stereo samples. All mono
samples are routed to stereo output and are panned as needed to fit the
overall stereo profile of the kit.

This kit has been tested with [sfizz](https://sfz.tools/sfizz/)

## Quick setup with Ardour + sfizz

* Create a new midi track, name it something like "Drum Kit", select
  Instrument: sfizz-multi.
* In the Plugin Setup dialog, select Output Configuration: 10 Channels, and
  Enable Fan out.
* Open the sfizz-multi plugin on the track, load the `full_kit.sfz` file.
* Rename the output busses in order:
    * Overheads
    * Kick
    * Snare
    * Toms
    * Hihat
* Have fun

## Advanced usage

Edit keymap.sfz to customize the midi note mapping.

To use multiple stereo instances of sfizz instead of sfizz-multi, load the
following files:
* `overheads.sfz`
* `kick.sfz`
* `snare.sfz`
* `toms.sfz`
* `hihat.sfz`

## License

The creation of music using tchackpoum-sfz is allowed under the terms of the
[CC0](https://creativecommons.org/publicdomain/zero/1.0/) license.

The creation of derivative virtual drum kits is allowed under the terms of the
[CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) license.
Specifically, any modified or derivative drum kit using these samples must
credit Vincent Sermone as having originally recorded the samples, and must
itself be licensed under the same terms.
