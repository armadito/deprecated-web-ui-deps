# armadito-web-ui-deps
Deps for armadito-web-ui recipe build on launchpad

- This repository is merged during git build recipe on launchpad server.
- It is needed because downloading bower components is not possible during launchpad source package building.
- It would have been better if node_modules and bower_components where installable by apt.

See : https://answers.launchpad.net/launchpad/+question/292654


# Instructions for updating depencies

- $ ./autogen.sh
- $ ./configure
- $ make all
- commit and push on branch master
- travis-ci build will call launchpad code-import for synchronization with launchpad repo
