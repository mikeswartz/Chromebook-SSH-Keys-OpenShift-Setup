# Chromebook-SSH-Keys-OpenShift-Setup
Get your Chromebook to use SSH keys to allow access to your OpenShift account.  If you have a Chromebook and want to SSH into a server, here's the quick and dirty steps.

1. Setup Chromebook in Developer mode (Secure Shell won't allow new Chromebooks to upload SSH keys, you need to use Developer Mode's shell prompt).
2. Launch terminal: ctrl+alt+t in the Chrome browser
3. At terminal prompt type "shell" and hit enter
4. Create ssh keys
    https://help.github.com/articles/generating-ssh-keys
5. Run eval "$(ssh-agent)" to launch ssh-agent
    http://unix.stackexchange.com/questions/48863/ssh-add-complains-could-not-open-a-connection-to-your-authentication-agent/48868#48868
6. Add your SSH keys to your Chromebook's SSH command
    "ssh-add ~/.ssh/key-name"
7. Add your public key contents to your server you wish to SSH into.
8. In the Chromebook terminal, SSH to your server and enter the pass phrase you created with for your SSH keys.﻿
