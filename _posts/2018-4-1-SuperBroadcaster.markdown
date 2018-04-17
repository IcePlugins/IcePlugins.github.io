---
layout: post
title: SuperBroadcaster
description: 'Allows you to do timed or manual broadcasts using UI effects. Some text will stay on the top of a player''s screen when a superbroadcast is created.'
download: 'https://github.com/IcePlugins/SuperBroadcaster/releases'
github: 'https://github.com/IcePlugins/SuperBroadcaster/'
documentation_block: |
  <?xml version="1.0" encoding="utf-8"?>
  <SuperBroadcasterConfiguration xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <!-- Duration of manual broadcast if a time is not specified. -->
    <defaultBroadcastDuration>5</defaultBroadcastDuration>
    <!-- Time limit for manual broadcasts. -->
    <broadcastTimeLimit>25</broadcastTimeLimit>
    <!-- ID of the broadcast effect. If you are using my assets, DO NOT CHANGE THIS. -->
    <effectId>42069</effectId>
    <!-- How often a timed broadcast should repeat. Set this to 0 to disable timed broadcasts. -->
    <repeatingBroadcastInterval>10</repeatingBroadcastInterval>
    <!-- How long a timed broadcast should stay on screen. -->
    <repeatingBroadcastStayTime>5</repeatingBroadcastStayTime>
    <!-- Messages for timed broadcasts. -->
    <broadcastMessages>
      <!-- Message for your timed broadcast. -->
      <message>SupahBroadcasto!!!!</message>
      <message>This is a SUPER broadcast!</message>
      <message>set repeatingBroadcastInterval to -1 to disable this!</message>
    </broadcastMessages>
  </SuperBroadcasterConfiguration>

commands:
    - name: '/superbroadcast "your message" &lt;time&gt;'
      doc: 'Superbroadcast command. Replace "your message" with your message, quotes included. Replace &lt;time&gt; with the time in seconds that the broadcast should stay on screen. Aliases: /sb and /sbroadcast. Requires superbroadcast.broadcast.<br><a href="https://docs.unity3d.com/Manual/StyledText.html">Supports RICH TEXT</a>'

permissions:
    - name: superbroadcast.broadcast
      doc: 'Gives a player access to the /superbroadcast command.'
---
<b>NOTICE:</b>
Requires my assets pack to be installed on the server. Can be downloaded from the Steam Workshop:
<br>
<a href="http://steamcommunity.com/sharedfiles/filedetails/?id=1349772817">http://steamcommunity.com/sharedfiles/filedetails/?id=1349772817</a>