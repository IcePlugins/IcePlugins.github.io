---
layout: post
title: ExtraRestrictor
description: 'Item restriction plugin using events instead of continuous checks for no lag and with support for group based restrictions.'
download: 'https://github.com/IcePlugins/ExtraRestrictor/releases'
github: 'https://github.com/IcePlugins/ExtraRestrictor'
documentation_block: |
  <?xml version="1.0" encoding="utf-8"?>
  <ExtraRestrictorConfiguration xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <!-- List of restricted items by ID -->
    <Restricted>
      <!-- Single restricted item. Use the "BypassPermissions" attribute to assign a permission that would allow a user to bypass this restriction. -->
      <Item BypassPermission="bypass.explosives">519</Item>
      <!-- Don't want to use a BypassPermission? No problem, simply exclude it from the element. -->
      <Item>1441</Item>
    </Restricted>
    <!-- Ignore admins or not -->
    <IgnoreAdmins>true</IgnoreAdmins>
  </ExtraRestrictorConfiguration>

permissions:
    - name: extrarestrictor.bypass
      doc: 'Allows a player to bypass all item restrictions.'
    - name: Custom
      doc: 'You can define a custom bypass restriction for certain items. Look in the configuration documentation on this page for an example.'
---
