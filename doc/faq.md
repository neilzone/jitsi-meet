**1. How to tell if my server instance is behind NAT?**

A. In general, if the tool ifconfig (or ipconfig) shows the assigned IP address to be some local address (10.x.x.x or 192.x.x.x) but you know that its public IP address is different from that, the server is most probably behind NAT

**2. Clients could communicate well in room created at meet.jit.si . The same clients still could connect to my self-hosted instance but can neither hear nor see one another. What's wrong?**

A. Most probably, the server is behind NAT. See this [resolved question](https://community.jitsi.org/t/cannot-see-video-or-hear-audio-on-self-hosted-instance/). You need to follow the steps detailed [here](https://github.com/jitsi/jitsi-meet/blob/master/doc/quick-install.md#Advanced-configuration)

**3. How can I protect my meetings with jitsi?**

If you are using the hosted meet.jit.si platform:

_1.) Create a "strong" room name._

Use a strong room name, which no-one else is likely to be using. Use the name generator on the welcome page, or else generate your own "strong" name.

For example, on macOS, in terminal, you can use `uuidgen` to generate a string of letters of numbers (e.g. B741B63E-C5E6-4D82-BAC4-048BE25D8CC7).

Your room name would be meet.jit.si/B741B63E-C5E6-4D82-BAC4-048BE25D8CC7

If you use "test" or "LucysMeeting" or "pilates" or similar, then it's highly likely that other users will have had the same idea.

_2.) Use a different room name for each meeting / conference you have._

If you are going to have multiple meetings, ideally use a different room name for each one.

If that is not practical, at least use a different room name for each group of people.

_3.) Add a password to the room._

Once you have started your room, set a password for it. Only people who have the password can join from that point on, but it does not affect people who have already joined.

You will need to tell everyone the password.

If they give the password to others, those other people can also join.


If you are using your own instance of jitsi:

In addition to the tips above, consider enabling the ["secure domain" configuration](https://github.com/jitsi/jicofo#secure-domain). This requires you (or someone else) to enter a username and password to open a room.


