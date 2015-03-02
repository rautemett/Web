---
layout: page
title: IRC
permalink: /irc/
---

mettBot: [github](http://github.com/Ro0mquy/MettBot) \\
Log seit immer™: Komm doch lieber in den Channel \\
<!-- #mett Stats: [mett.html (mett/salami)](https://mett:salami@excalibur.h4ndi.de/~hendrik/ircstats/mett.html) -->

## Server

### irc.thw23.de

Host: irc.thw23.de \\
Ports: 2342, 4223 (SSL) \\
Admins: samohT, izibi \\
SHA1 Fingerprint: 35:DB:AA:EB:4C:B3:6A:2C:2F:8B:CF:3F:71:FC:14:2A:84:B7:7B:2A [(Zertifikat)](https://julian.taurus.uberspace.de/ircmett/certs/irc.thw23.de.pem)

### irc.kurz.pw

Host: irc.kurz.pw \\
Ports: 6667, 6697 (SSL) \\
Admins: lukas2511, izibi \\
SHA1 Fingerprint: E4:52:39:34:A9:07:8B:6A:B3:6D:BA:CB:7D:B9:8C:E9:BF:02:A5:ED [(Zertifikat)](https://julian.taurus.uberspace.de/ircmett/certs/trollkampf.luma-hosting.de.pem)

### irc.ps0ke.de

Host: irc.ps0ke.de \\
Ports: 2342 \\
Admin: Ps0ke \\
SHA1 Fingerprint: 21:92:EB:6B:DC:40:DD:07:C8:C5:56:81:25:06:87:02:02:FC:75:17 [(Zertifikat)](https://julian.taurus.uberspace.de/ircmett/certs/irc.ps0ke.de.pem)

### irc.0x4a42.net

Host: irc.0x4a42.net \\
Ports: 6667, 2342, 6697 (SSL), 4223 (SSL) \\
Admin: izibi \\
SHA1 Fingerprint: D0:9F:2C:38:61:6D:82:7E:6F:17:C4:4D:14:9D:99:3E:E2:3D:11:EE [(Zertifikat)](https://julian.taurus.uberspace.de/ircmett/certs/irc.0x4a42.net.pem)

### irc.firebird.io

Host: irc.firebird.io \\
Ports: 6667, 6697 (SSL) \\
Admin: firebird \\
SHA1 Fingerprint: F8:0C:E0:EC:11:D0:6B:9A:A4:A9:BA:65:01:31:57:F6:66:2F:F3:60 [(Zertifikat)](https://firebird.io/certificate.pem)

## Map

![IRCMap](https://julian.taurus.uberspace.de/ircmett/map.png)

([ASCII-Version](https://julian.taurus.uberspace.de/ircmett/map.txt))

## irssi

{% highlight irc %}
/network add IRCmett
/server add -network IRCmett -ssl ssl.ircmett.de 4223
/channel add -auto #mett IRCmett
/connect IRCmett
{% endhighlight %}

## Server Config

{% highlight ini %}
[Global]
Name = ...
AdminInfo1 = ...
AdminInfo2 = ...
AdminEMail = ...
Info = ...
MotdFile = ...
Ports = ...

[SSL]
CertFile = ...
DHFile = ...
KeyFile = ...
KeyFilePassword = ...
Ports = ...

[Limits]
ConnectRetry = 60
MaxConnections = 0
MaxConnectionsIP = 5
MaxNickLength = 15
PingTimeout = 120
PongTimeout = 120

[Options]
AllowRemoteOper = yes
ConnectIPv6 = yes
ConnectIPv4 = yes
DNS = yes
Ident = yes
NoticeAuth = yes
OperCanUseMode = yes
OperChanPAutoOp = yes

[Operator]
Name = ...
Password = ...

[Server]
Name = ...
Host = ...
Port = ...
MyPassword = ...
PeerPassword = ...
SSLConnect = yes
{% endhighlight %}
