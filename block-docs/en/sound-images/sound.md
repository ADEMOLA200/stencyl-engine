# palette.sounds.sound

> Read our [Sounds]($pedia/playing-sounds-and-music/) article for an explanation of these blocks.

# play-sound4 -- Play / Loop Sound

Plays (or loops) the chosen sound on the next available channel.

# stop-sounds -- Stop all Sounds

Immediately stops playback of all sounds.

# set-volume -- Set Volume

Sets the global sound volume level. Individual channels maintain their own volume level, which is multiplied against the global volume level. Specify a value between [0-100] inclusive.

# fade-sounds -- Fade Volume In / Out

Fades the global sound volume level in (to 100%) or out (to 0%) over time, given in seconds.

# fade-sounds-percent -- Fade Volume to Percent

Fades global volume to the given percent.

# play-sound-channel -- Play / Loop Sound on Channel

Plays (or loops) a sound on the specified channel. If one was previously playing on the channel, it stops and gets replaced.

# control-sound-channel -- Stop / Pause / Resume Sound on Channel

Controls playback of a sound on the specified channel (if one is playing). Stopping a sound and resuming will force it start from the beginning.

# set-volume-channel -- Set Volume on Channel

Sets the volume level for the specified channel, which is multiplied against the global volume level. Specify a value between [0-100] inclusive.

# fade-sound-channel -- Fade Volume In / Out on Channel

Fades the sound volume level for the specified channel in (to 100%) or out (to 0%) over time. Duration is given in seconds.

# fade-sound-channel-percent -- Fade Volume to Percent on Channel

Fades channel volume to the given percent.

# set-panning-channel -- Set Panning on Channel

Sets the panning of a channel (negative 100% is far left, positive 100% is far right).

# set-position-channel -- Set Position on Channel

Set position for sound on a specific channel in milliseconds.

# get-position-channel -- Sound Position on Channel

Returns the current playback position of the sound on the specified channel in milliseconds.

# get-length-channel -- Length of Track on Channel

Returns the length of the sound on the specified channel in milliseconds.

# palette.sounds.sound.sounds -- ""

# get-length-sound -- Length of Sound

Returns the length of the specified sound in milliseconds.

# text-to-sound -- Get Sound with Name

Returns a sound, given its name.