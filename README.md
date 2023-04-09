# G729-Codec-For-Freeswitch
After searching for the free G729 Codec that is compatible with Freeswitch I have finally found it

How to install G729 Free Codec on FreeSWITCH

1. Download mod_bcg729.so from here.

2. Place the g729 codec into FreeSWITCH modules directory
   <br>Copy mod_bcg729.so file to <code>/usr/lib/freeswitch/mod</code> 
   
3. Open FreeSWITCH Command-Line Interface: <code>#fs_cli</code>

4. Load the mod_bcg729 module: <code>freeswitch@"yourswitchname"> load mod_bcg729</code>

5. Add G729 to your global_codec_prefs/outbound_codec_prefs in FusionPBX/Astpp

6. Restart FreeSWITCH: <code>fsctl shutdown restart</code> (N.B restarting your switch might unload the newly loaded bcg729 codec, always double check it)


That’s it now you can use codec g729 in calls and transcoding.

<br>
<i>*Disclaimer: This is not my work, merely sharing what I found from a repo that went missing in 2020.</i>
