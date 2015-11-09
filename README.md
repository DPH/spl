# spl
Control Sonos playlists.

This utility controls Sonos playlists including backup and restore.

Here are the options:

```
usage: spl.py [-h] [-l] [-S] [-x PLAYLIST] [-X] [-f] [-i FILE] [-s SPEAKER]
              [-P] [-p] [-q PLAYLIST] [-m PLAYMODE] [-t]

Utility for Sonos playlists including backup and restore. The backup file is
XSPF format and is stored in the current directory. For import, the name of
the playlist is stored in the XSPF file, it is not the name of the file.

optional arguments:
  -h, --help            show this help message and exit
  -l, --listPlaylist    List the playlists.
  -S, --listSpeakerInfo
                        List information about the speakers.
  -x PLAYLIST, --exportPlaylist PLAYLIST
                        Export the playlist.
  -X, --exportAllPlaylists
                        Export all playlists.
  -f, --force           Force overwrite of export files.
  -i FILE, --importPlaylistFile FILE
                        Import the playlist file.
  -s SPEAKER, --speaker SPEAKER
                        Speaker name or IP address.
  -P, --partyModeOn     Use all speakers. Must be used with -s to designate
                        the group coordinator.
  -p, --partyModeOff    Stop party mode.
  -q PLAYLIST, --replaceQueue PLAYLIST
                        Replace queue with playlist. Speakers must be in party
                        mode or option -s is required.
  -m PLAYMODE, --playMode PLAYMODE
                        Play mode: SRF, S = shuffle on, R = repeat on, F =
                        cross fade on. Lower case is off. Default is SRf.
  -t, --togglePausePlay
                        Toggle pause/play.
```

#####Dependencies

This utility uses the SoCo module version 0.11.1 (https://github.com/SoCo/SoCo) to control the Sonos speakers.  SoCo is available via pip, see the web page for details. Spl was written for Python 2.7.

