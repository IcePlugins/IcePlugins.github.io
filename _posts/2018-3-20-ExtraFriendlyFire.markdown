---
layout: post
title: ExtraFriendlyFire
description: 'Prevents members of the same RocketMod group from firing on each other.'
download: 'https://github.com/IcePlugins/ExtraFriendlyFire/releases'
github: 'https://github.com/IcePlugins/ExtraFriendlyFire/'
documentation_block: |
    <?xml version="1.0" encoding="utf-8"?>
    <ExtraFriendlyFireConfig xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <!-- List of groups to prevent friendly fire. -->
    <groups>
        <!-- Single group. If a player is in this group and tries to damage another player in the same group, no damage will be dealt. Damage will still be dealt to players of other groups. -->
        <group>default</group>
        <group>VIP</group>
        <group>Moderator</group>
        <group>NoDamageGroup</group>
    </groups>
    <!-- If the plugin will ignore admins or not -->
    <ignoreAdmin>true</ignoreAdmin>
    <!-- If the player has this permission, the plugin will ignore them. -->
    <ignorePermissionString>extrafriendlyfire.ignore</ignorePermissionString>
    </ExtraFriendlyFireConfig>
---
