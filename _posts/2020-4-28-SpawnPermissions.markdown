---
layout: post
title: SpawnPermissions
description: |
  Restrictions on /i and /v based on permissions. Works on administrators. Cooldowns only trigger when the command is successful.
   This plugin is created and maintained by Kr4ken-9 and licensed under the GNU General Public License v3.0.
  https://github.com/Kr4ken-9
download: 'https://github.com/IcePlugins/SpawnPermissions/releases'
github: 'https://github.com/IcePlugins/SpawnPermissions/'
documentation_block: |
  <?xml version="1.0" encoding="utf-8"?>
  <Configuration xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
    <!-- If enabled, players will only be able to spawn vehicles that are whitelisted with the correct permission -->
    <EnableVehicleWhitelist>false</EnableVehicleWhitelist>
    <!-- If enabled, players can spawn any vehicle except those blacklisted with the correct permission -->
    <EnableVehicleBlacklist>false</EnableVehicleBlacklist>
    <!-- If enabled, players will only be able to spawn specific items that are whitelisted with the correct permission -->
    <EnableItemWhitelist>false</EnableItemWhitelist>
    <!-- If enabled, players can spawn any item except those blacklisted with the correct permission -->
    <EnableItemBlacklist>false</EnableItemBlacklist>
    <!-- If enabled, players won't have a cooldown for /i or /v when they try to spawn a blacklisted/not whitelisted item or vehicle -->
    <WaiveCooldowns>false</WaiveCooldowns>
    <!-- If enabled, admins will still have blacklisted/whitelisted items/vehicles unless they have the bypass permission -->
    <OverrideAdmin>false</OverrideAdmin>
  </Configuration>
permissions:
    - name: spawnpermissions.v.blist.{ID}
      doc: 'Causes the vehicle to be blacklisted for the permission group'
    - name: spawnpermissions.v.wlist.{ID}
      doc: Causes the vehicle to be whitelisted for the permission group
    - name: spawnpermissions.i.blist.{ID}
      doc: Causes the item to be blacklisted for the permission group
    - name: spawnpermissions.i.wlist.{ID}
      doc: Causes the item to be whitelisted for the permission group
    - name: spawnpermissions.bypass
      doc: Anyone with this permission can spawn any item/vehicle
---
