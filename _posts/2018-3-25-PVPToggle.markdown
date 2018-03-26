---
layout: post
title: PVPToggle
description: 'Allows players to individually toggle their PVP on/off, along with UI effects to show if a player is invulnerable and if the player is in PVP.'
download: 'https://github.com/IcePlugins/PVPToggle/releases'
github: 'https://github.com/IcePlugins/PVPToggle/'
documentation_block: |
  <?xml version="1.0" encoding="utf-8"?>
  <PvpToggleConfiguration xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <!-- If a player should enter the server in PVE mode -->
    <pveByDefault>false</pveByDefault>
    <!-- If the plugin should ignore admins -->
    <ignoreAdmins>false</ignoreAdmins>
    <!-- If a warning effect is enabled. Requires the workshop mod. -->
    <enableWarningEffect>true</enableWarningEffect>
    <!-- Warning effect ID. Default value (60125) is the ID of my effect. Leave unchanged unless you are using your own. -->
    <warningEffectId>60125</warningEffectId>
    <!-- How long after a warning effect pops up until it can pop up again -->
    <warningCooldown>3</warningCooldown>
    <!-- How long the warning effect stays on screen -->
    <warningScreentime>2</warningScreentime>
    <!-- If an indicator text to display in the top right corner will be shown. Requires the workshop mod. -->
    <enableIndicatorEffect>true</enableIndicatorEffect>
    <!-- If the indicator is enabled on server join -->
    <indicatorByDefault>true</indicatorByDefault>
    <!-- Indicator Effect ID. Default value (60125) is the ID of my effect. Leave unchanged unless you are using your own. -->
    <indicatorEffectId>60126</indicatorEffectId>
  </PvpToggleConfiguration>
commands:
    - name: /pvp
      doc: 'Toggles your own PVP mode on/off. Requires pvptoggle.pvp.'
    - name: /pvp [player]
      doc: 'Displays a player''s PVP status. Requires pvptoggle.pvp.'
    - name: /indicator
      doc: 'Turns the PVP indicator on/off. Requires pvptoggle.indicator.'

permissions:
    - name: pvptoggle.pvp
      doc: 'Allows a player use /pvp'
    - name: pvptoggle.indicator
      doc: 'Allows a plyer to use /indicator'
    - name: pvptoggle.bypass
      doc: 'A player with this permission will bypass the PVP/PVE check.'
---
<b>NOTICE:</b>
<br>
Requires my assets pack to be installed on the server. 
<br>
<b><a href="http://steamcommunity.com/sharedfiles/filedetails/?id=1341952069">http://steamcommunity.com/sharedfiles/filedetails/?id=1341952069</a></b>