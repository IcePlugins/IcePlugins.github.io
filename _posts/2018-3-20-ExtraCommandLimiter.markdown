---
layout: post
title: ExtraCommandLimiter
description: 'A plugin that allows you to limit command usage to inside or outside of safezones or deadzones.'
download: 'https://github.com/ExtraConcentratedJuice/ExtraCommandLimiter/releases'
github: 'https://github.com/ExtraConcentratedJuice/ExtraCommandLimiter/'
documentation_block: |
    <?xml version="1.0" encoding="utf-8"?>
    <ExtraCommandLimiterConfiguration xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <!-- Commands blocked in safezone -->
    <safezoneBlockedCommands>
        <!-- Single command, case is not sensitive. -->
        <string>vault</string>
    </safezoneBlockedCommands>
    <!-- Commands blocked in deadzone -->
    <deadzoneBlockedCommands>
        <string>spaghetti</string>
    </deadzoneBlockedCommands>
    <!-- Only allow these commands inside of a safezone -->
    <safezoneOnlyCommands>
        <string>vault</string>
    </safezoneOnlyCommands>
    <!-- Only allow these commands inside of a deadzone -->
    <deadzoneOnlyCommands>
        <string>meme</string>
    </deadzoneOnlyCommands>
    <!-- Allow admins to bypass the check -->
    <allowAdminOverride>true</allowAdminOverride>
    <!-- Any player that has this permission will be ignored -->
    <ignorePlayerPermission>ExtraCommandLimiter.ignore</ignorePlayerPermission>
    </ExtraCommandLimiterConfiguration>'
---

Requires you to install a library. More details available on the download page.
