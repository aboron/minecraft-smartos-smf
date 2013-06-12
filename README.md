minecraft-smartos-smf
=====================

Minecraft server SMF manifest and service helper scripts for SmartOS (Solaris)

To use:

1) Make sure your mincraft folder is the same as the scripts assume "/opt/local/minecraft" (or change them).

2) Symlink the bin files from custom/bin into the path listed in custom/smf/minecraft.xml somewhere (/opt/local/bin is good).

3) Install tmux: pkgin in tmux

4) Create the minecrft user and group.

5) svccfg import minecraft.xml

6) svcadm enable minecraft

7) Use mc-attach when you need console access ('Ctrl-b' then 'd' to exit console).

Enjoy!


Comments, additions, corrections and suggestions are welcome.

I will be extending the functionality as time permits.

TODO:

1. Put all the variables into svcprops and reference those from the mc-console and mc-service scripts.
2. Write an update script.
3. Write an installer script.

Check my blog post on the creation of this package:

http://greggaskill.us/2013/06/minecraft-on-smartos
