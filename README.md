# G729-Codec-For-Freeswitch
After searching for the free G729 Codec that is compatible with Freeswitch I have finally found it

How to install G729 Free Codec on FreeSWITCH

1. Download mod_bcg729.so from here.

2. Place the g729 codec into FreeSWITCH modules directory
   Copy mod_bcg729.so file to /usr/lib/freeswitch/mod directory
   
3. Open FreeSWITCH Command-Line Interface: #fs_cli

4. Load the mod_bcg729 module: freeswitch@"yourswitchname"> load mod_bcg729

5. Add G729 to your global_codec_prefs/outbound_codec_prefs in FusionPBX/Astpp

6. Restart FreeSWITCH: fsctl shutdown restart


That’s It now you can use codec g729 in calls and transcoding.


Disclaimer: This is not my work, merely sharing what I found from a repo that went missing in 2020.
