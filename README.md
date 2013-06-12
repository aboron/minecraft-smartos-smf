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

<p xmlns:dct="http://purl.org/dc/terms/" xmlns:vcard="http://www.w3.org/2001/vcard-rdf/3.0#">
  <a rel="license"
     href="http://creativecommons.org/publicdomain/zero/1.0/">
    <img src="http://i.creativecommons.org/p/zero/1.0/88x31.png" style="border-style: none;" alt="CC0" />
  </a>
  <br />
  To the extent possible under law,
  <a rel="dct:publisher"
     href="http://greggaskill.us">
    <span property="dct:title">Gregory Gaskill</span></a>
  has waived all copyright and related or neighboring rights to
  <span property="dct:title">minecraft-smartos-smf</span>.
This work is published from:
<span property="vcard:Country" datatype="dct:ISO3166"
      content="US" about="greggaskill.us">
  United States</span>.
</p>

See LICENSE for more details.