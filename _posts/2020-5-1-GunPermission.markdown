---
layout: post
title: GunPermission
author: hiilikewiki56
license: GPL-3.0
license_url: https://www.gnu.org/licenses/gpl-3.0.en.html
description_short: GunPermission requires players to have a permission to equip guns. Certain guns can be blacklisted.
description: |
  GunPermission requires players to have a permission to possess guns. Certain guns can be blacklisted.
  <br />
  <br />
  This plugin is created by hiilikewiki56 and licensed under the GNU General Public License v3.0.
  <br />
  <br />
  <a href="https://github.com/archie426">https://github.com/archie426</a>
download: 'https://github.com/IcePlugins/GunPermission/releases'
github: 'https://github.com/IcePlugins/GunPermission/'
documentation_block: |
  <?xml version="1.0" encoding="utf-8"?>
  <GunPermissionConfiguration xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
    <!-- List of permissions that lets a player possess guns -->
    <Permissions>
      <string>gunpermission.gunsallowed</string>
    </Permissions>
    <!-- List of gun IDs that any player cannot possess -->
    <BlacklistedGunIds>
      <unsignedShort>297</unsignedShort>
    </BlacklistedGunIds>
  </GunPermissionConfiguration>
---
