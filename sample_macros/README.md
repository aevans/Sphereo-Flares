Sample Macros
=============

- - - -

MacroLab Macro: __solarflare1__

> solarflare1[] = { ID, FLAGS, 0x20, 0x00, 0x1c, 0x54, 0x75, 0x72, 0x6e, 0x20, 0x6f, 0x66, 0x66, 0x20, 0x6d, 0x6f, 0x74, 0x6f, 0x72, 0x20, 0x73, 0x74, 0x61, 0x62, 0x69, 0x6c, 0x69, 0x7a, 0x61, 0x74, 0x69, 0x6f, 0x6e, 0x03, 0x00, 0x00, 0x20, 0x00, 0x1f, 0x43, 0x79, 0x63, 0x6c, 0x65, 0x20, 0x74, 0x68, 0x72, 0x6f, 0x75, 0x67, 0x68, 0x20, 0x72, 0x65, 0x64, 0x2f, 0x6f, 0x72, 0x61, 0x6e, 0x67, 0x65, 0x20, 0x63, 0x6f, 0x6c, 0x6f, 0x72, 0x73, 0x1e, 0x05, 0x07, 0xd4, 0x1e, 0x00, 0x00, 0x0b, 0x00, 0x64, 0x07, 0xd5, 0x0f, 0x00, 0x00, 0x0b, 0x00, 0x64, 0x07, 0xd6, 0x00, 0x00, 0x00, 0x0b, 0x00, 0xc8, 0x1f, 0x0b, 0x01, 0xc2, 0x1e, 0x14, 0x07, 0xd4, 0x2d, 0x00, 0x00, 0x0b, 0x00, 0x96, 0x07, 0xd6, 0x00, 0x00, 0x00, 0x0b, 0x00, 0x96, 0x1f, 0x0b, 0x01, 0x77, 0x1e, 0x06, 0x07, 0xd0, 0x3f, 0x00, 0x00, 0x0b, 0x00, 0xaf, 0x07, 0xd6, 0x0f, 0x00, 0x00, 0x0b, 0x00, 0xaf, 0x1f, 0x0b, 0x01, 0x2c, 0x20, 0x00, 0x06, 0x52, 0x65, 0x70, 0x65, 0x61, 0x74, 0x0c, 0x00, 0x00 };


The __solarflare1__ macro was hand built using the `Sphero MacroLab` app.  It is intended to mimic the pulses of solar activity from the following STEREO movie.  (Chances are it still needs work, but it's a close enough approximation for an example file.)

[http://stereo.gsfc.nasa.gov/gallery/item.php?id=selects&iid=122](http://stereo.gsfc.nasa.gov/gallery/item.php?id=selects&iid=122)

- - - -

MacroLab Macro: __solar_flare__

> solar_flare[] = { ID, FLAGS, 0x03, 0x00, 0x00, 0x1e, 0x0a, 0x07, 0x00, 0x7f, 0xff, 0x00, 0x14, 0x00, 0x00, 0xff, 0x01, 0xf4, 0x0b, 0x01, 0xf4, 0x1f, 0x07, 0x00, 0x56, 0xff, 0x00, 0x0b, 0x00, 0x64, 0x1e, 0x05, 0x1f, 0x0b, 0x00, 0x64, 0x03, 0x01, 0x00, 0x1e, 0x05, 0x09, 0x00, 0x00, 0x07, 0x00, 0x7f, 0xff, 0x00, 0x14, 0x00, 0x00, 0xff, 0x01, 0x2c, 0x09, 0x7f, 0x00, 0x1a, 0x00, 0x0f, 0x00, 0x96, 0x0b, 0x00, 0x96, 0x1a, 0xff, 0xf1, 0x00, 0x96, 0x09, 0xff, 0x00, 0x0b, 0x00, 0x96, 0x1f, 0x03, 0x00, 0x00, 0x09, 0x00, 0x00, 0x07, 0x00, 0x56, 0xff, 0x00, 0x0b, 0x00, 0x64, 0x1e, 0x0a, 0x07, 0x00, 0x00, 0xff, 0x00, 0x14, 0x00, 0x7f, 0xff, 0x01, 0xf4, 0x0b, 0x01, 0xf4, 0x1f, 0x07, 0x00, 0x00, 0xff, 0x00, 0x0b, 0x00, 0x64, 0x0c, 0x00, 0x00 };


The __solar_flare__ macro uses the color Fade command instead of setting a series of color changes.  It also represents a solar flare event by pulsing the tail light while rotating in place left and right about 15 degrees in each direction.  It is not modeled after any specific time series data, but is setup with multiple loops.  Each loop count can be changed along with the RGB start and fade-to colors.  The duration of the delay commands inside the loop should match the total duration of the fade command.  Use each of the separate loops to mimic the time series data of solar flare activity, or set their values to 0 if they aren't needed.

This macro introduces additional feedback for solar flare activity and is not meant to represent any specific set of solar flare activity data.

- - - -

MacroLab Macro: __sleep__

> sleep[] = { ID, FLAGS, 0x0e, 0x00, 0x00, 0x00 };


The __sleep__ macro is included to allow putting the Sphero to sleep from within the Sphero MacroLab app instead of having to switch to the main Sphero app or return it to it's base station.

- - - -


Usage:
------

Email a copy of the .sphero file(s) to an account you can access on your mobile device with the `Sphero MacroLab` app.  Click or select the attachment to open it using the `Sphero MacroLab` app.

