# Atmosphere

A Python script for mixing looped white noise-ish sounds.


## Installation

1. Put `atmosphere` somewhere in your `$PATH`. You may also want to edit the
`CONFIG_PATH`.
2. Create a directory and put some sound files in it.
3. Create a config file that looks something like this:

```
# Sound path
/path/to/that/directory/with/sound/files

# Volumes (>1 = louder, <1 = quieter)
# Don't include extension
brook 0.3
crickets 0.9
fireplace 1.2
forest_rain 1.1
thunder1 1.3
thunder2 1.3
waves 0.05
wind 1.2
```

No extensions needed on the filenames. Sox can handle most common formats
(.wav, .mp3, .flac, etc.).

The numbers after the filenames are gain levels. Set it to 1.0 to leave it
as-is; greater than 1 to make it louder; and less than 1 to make it quieter.


## Usage

Assuming it's in your path, just run it: `atmosphere` (and then ctrl+c to exit
when you're done).


## Dependencies

- Install Sox. (Atmosphere uses its `play` command.)
