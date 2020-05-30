---
layout: post
title: CopiedLobbyMess
author: AtiLion
license: GPL-3.0
license_url: https://www.gnu.org/licenses/gpl-3.0.en.html
description_short: Messes with the server information presented when you click on the server in the multiplayer menu. Modify plugins, etc.
description: |
  Messes with the server information presented when you click on the server in the multiplayer menu. Can make RocketMod invisible, modify workshop items, hide plugins, and a bunch of other cool stuff.
  <br />
  <br />
  This plugin is created by AtiLion and licensed under the GNU General Public License v3.0.
  <br />
  <br />
  <a href="https://github.com/AtiLion">https://github.com/AtiLion</a>
download: 'https://github.com/IcePlugins/CopiedLobbyMess/releases'
github: 'https://github.com/IcePlugins/CopiedLobbyMess/'
documentation_block: |
  <?xml version="1.0" encoding="utf-8"?>
  <Configuration xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
    <Logging>true</Logging>
    <!-- Makes the server appear to be vanilla if set to true -->
    <InvisibleRocket>false</InvisibleRocket>
    <HidePlugins>false</HidePlugins>
    <!-- This should be true if you want to change your plugins. -->
    <MessPlugins>false</MessPlugins>
    <!-- Every line here is a line in your plugins box changed. -->
    <!-- Only used if MessPlugins is set to true. -->
    <Plugins>
      <string>Plugins removed by</string>
      <string>CopiedLobbyMess</string>
      <string>AtiLion is gay</string>
    </Plugins>
    <HideWorkshop>true</HideWorkshop>
    <!-- Same thing as above except for the workshop box. -->
    <MessWorkshop>false</MessWorkshop>
    <!-- Workshop item IDs to be put in the workshop box -->
    <Workshop>
      <string>936182532</string>
      <string>1112690830</string>
    </Workshop>
    <!-- Changes the gamemode -->
    <MessGamemode>false</MessGamemode>
    <Gamemode>Nothing you have ever seen before</Gamemode>
    <!-- Hides your game config -->
    <HideConfig>true</HideConfig>
    <!-- Modifies your game config if true -->
    <MessConfig>false</MessConfig>
    <IsPVP>true</IsPVP>
    <HasCheats>false</HasCheats>
    <!-- Use NORMAL, EASY, or HARD -->
    <Difficulty>NRM</Difficulty>
    <!-- Use FIRST, BOTH, THIRD, or VEHICLE -->
    <CameraMode>2Pp</CameraMode>
    <GoldOnly>false</GoldOnly>
    <HasBattleye>true</HasBattleye>
    <IsVanilla>false</IsVanilla>
  </Configuration>
---
