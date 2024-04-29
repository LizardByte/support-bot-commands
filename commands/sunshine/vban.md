# VBan

VBan is a microphone transmission protocol made by the makers of VB cable. It allows you to pass your microphone from
your client to your host on supported clients. You will need to download "Receptor" on your host and "Talkie" on your
clients. You can find both here: <https://vb-audio.com/Voicemeeter/vban.htm>

Once downloaded, extracted, and placed in your desired location, all you need to do is run them and do some minor
configuration as follows:

1. On Talkie, you give your stream a name (like the device name) and the IP address of the host.
   You may also have to go into settings via the menu button to assign a microphone.
2. On Receptor, you assign an audio output. You may have to install VB cable to make a digital one.
   Then click the stream name. The stream you made from Talkie should appear as an option.

That's it!

:information_source: **Notes**

- As Receptor does not auto-start as it is not an installed program, you may want to add it as a
  Sunshine pre-launch command. Receptor will remember the last audio stream it was connected to.
- You may have to configure Windows/Game audio setting on the host to use the Microphone if you are using VB cable.
- To use Vban over the internet, you will also have to manually forward UDP Port 6980.
