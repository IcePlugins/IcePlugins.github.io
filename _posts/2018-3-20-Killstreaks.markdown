---
layout: post
title: Killstreaks
description: 'Keep track of and give rewards for player killstreaks.'
download: 'https://github.com/IcePlugins/Killstreaks/releases'
github: 'https://github.com/IcePlugins/Killstreaks/'
documentation_block: |
  <?xml version="1.0" encoding="utf-8"?>
  <KillStreaksConfig xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <!-- Lets killstreaks persist over restarts. -->
    <enable_restart_persistence>true</enable_restart_persistence>
    <!-- Lets killstreaks persist over sessions. -->
    <remove_streak_on_disconnect>false</remove_streak_on_disconnect>
    <!-- Message for killstreak. {0} is for the player's name and {1} is for kill amount. -->
    <kill_streak_message>{0} IS ON A KILL STREAK! ({1} kills)</kill_streak_message>
    <!-- Explains itself. -->
    <kill_streak_message_color>magenta</kill_streak_message_color>
    <!-- If killCount/killDivisor = 0, then a killstreak message will appear. -->
    <kill_divisor>5</kill_divisor>
    <!-- Lowest killstreak the message will appear for. -->
    <kill_streak_threshold>5</kill_streak_threshold>
    <!-- The killstreak at which if the player dies, a message will display. -->
    <kill_streak_lost_threshold>25</kill_streak_lost_threshold>
    <!-- Message for killstreak lost. {0} is player name, {1} is kill count. -->
    <kill_streak_lose_message>{0} DIED AND LOST THEIR KILL STREAK OF {1}!</kill_streak_lose_message>
    <!-- Explains itself. -->
    <kill_streak_lost_message_color>red</kill_streak_lost_message_color>
    <!-- List of command groups that will be executed on a killstreak. -->
    <CommandGroups>
      <!-- Single group. You can paste this to create multiple command groups. -->
      <Group>
        <!-- All of these commands will be executed when the killstreak is recognized. -->
        <Commands>
          <!-- Single command. {0} is the player's DisplayName. -->
          <Command>/heal {0}</Command>
          <Command>/give {0} 8 1</Command>
          <Command>/say woah</Command>
        </Commands>
        <!-- Minimum range of kills for this commandgroup to be executed. -->
        <KillMin>4</KillMin>
        <!-- Maximum range of kills for this commandgroup to be executed. -->
        <KillMax>20</KillMax>
      </Group>
    </CommandGroups>
  </KillStreaksConfig>
commands:
    - name: /kills
      doc: 'Displays the caller''s current kills. Requires killstreaks.kills.'

permissions:
    - name: killstreaks.kills
      doc: 'Allows a player to call /kills.'
---
