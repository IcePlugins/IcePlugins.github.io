---
layout: post
title: AntiLock
description: 'AntiLock allows you to limit the amount of vehicles a player can lock based on their permission group.'
download: 'https://github.com/IcePlugins/AntiLock/releases'
github: 'https://github.com/IcePlugins/AntiLock/'
documentation_block: |
  <?xml version="1.0" encoding="utf-8"?>
  <AntiLockConfiguration xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <!-- Default amount of locks allocated if player has no lock permissions -->
    <defaultLocks>0</defaultLocks>
    <!-- If the plugin should ignore admins -->
    <ignoreAdmins>true</ignoreAdmins>
    <!-- If a message should be displayed when the player hits their lock cap -->
    <displayMaxlocksNotice>true</displayMaxlocksNotice>
    <!-- If a message should appear when the player locks a vehicle -->
    <displayLockNotice>true</displayLockNotice>
    <!-- Lock groups -->
    <lockGroups>
      <!-- Lock group -->
      <LockGroup>
        <!-- Permission that a player in this group should have -->
        <Permission>antilock.lock</Permission>
        <!-- Max vehicle locks that the player holding the permission gets -->
        <MaxLocks>5</MaxLocks>
      </LockGroup>
      <LockGroup>
        <Permission>antilock.biglock</Permission>
        <MaxLocks>10</MaxLocks>
      </LockGroup>
    </lockGroups>
  </AntiLockConfiguration>
commands:
    - name: /clearlocks [player (OPTIONAL)]
      doc: 'Lets the player clear their own locks, or another''s if an argument is provided. antilock.clearlocks is required for the command without a parameter, antilock.clearlocks.other is required for the command with the parameter.'

permissions:
    - name: antilock.clearlocks
      doc: 'Allows a player to unlock all of his own vehicles.'
    - name: antilock.clearlocks.other
      doc: 'Allows a player to unlock all of another player''s vehicles.'
    - name: Custom
      doc: 'See the configuration to set up your own lock permissions.'
---
