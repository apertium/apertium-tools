# apertium-tools

[Apertium][1] is a free/open-source platform for developing rule-based machine
translation systems.

This repository holds submodules to [Apertium tools][2] that supplement the
Apertium core and the language data.

To clone this repository with all its submodules, run

    git clone --recurse-submodules --shallow-submodules --depth 1 git@github.com:apertium/apertium-tools.git

(Change `--depth 1` to `--depth N` to get the last N commits.)

Most users should not commit directly to this repository. All Apertium
repositories with the topic `apertium-tools` are automatically updated in this
repository as submodules.

However, changes can be made to submodules in this repository after cloning it.
To make a commit to each changed submodule:

    git submodule foreach 'git commit -a -m <message>'
    git submodule foreach 'git push'

More information about using Git is [on the wiki][3]. More information about the
submodules is in the READMEs of those repositories under https://github.com/apertium.

[1]: https://wiki.apertium.org/
[2]: https://wiki.apertium.org/wiki/Tools
[3]: https://wiki.apertium.org/wiki/Using_Git
