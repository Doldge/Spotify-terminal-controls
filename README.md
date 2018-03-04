# Spotify Controls from Bash.

Testing on Debian 9.3 with Gnome

apt-get install qdbus

If you get errors when trying to run the sp-\* commands, you may want to consider installing d-feet and looking for the spotify command paths yourself.

Once you've cloned the repo, set up a symlink for each of the sp comands into /usr/local/bin
i.e.

ln -s ~/spotify-commands/sp-\* /usr/local/sbin/

You may also want to consider setting up aliases.
i.e.

alias spn='sp-next'
alias spl='sp-prev'


Notes: sp-prev runs the previous command twice, as if the song is already playing, running the command once will only skip you back to the start of the song.
If you want to just manually run the command twice yourself you can use the sp-previous command instead (it runs the prev command only once).

