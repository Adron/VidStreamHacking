<> [README.md](README.md) <> ...

# Gotchas for Windows

* Windows OBS routinely doesn't show web content with the *Windows Capture* source option nor Display Capture.
* Be sure to setup audio before hand via the audio settings, don't add speaking audio via the input/output options in sources but instead via the Mixer instead. The others often have lag in the audio and create a poor experience.

# Gotchas for MacOS

* The audio is an oddball on MacOS, be sure to setup the """ plugin for adding audio from the machine itself, in other works to pick up video chat audio, game audio, or application audio itself from the machine this plugin is needed.

# Gotchas for Linux 

* None yet, got any, throw in a pull request!  :)
* Sometimes "Browser Source" isn't available. It appears that one possible solution is to install the plugin manually [here](https://github.com/bazukas/obs-qtwebkit).
