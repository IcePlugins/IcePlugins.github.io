---
layout: post
title: Colorize
description: 'Colorize allows players to change their chat color on the fly.'
download: 'https://github.com/IcePlugins/Colorize/releases'
github: 'https://github.com/IcePlugins/Colorize/'
documentation_block: |
    <?xml version="1.0" encoding="utf-8"?>
    <ColorizeConfig xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <!-- List of banned colors -->
    <banned_colors>
        <!-- Single banned color value in hex or UnityEngine color -->
        <color>#FFFFFF</color>
        <color>#FFF000</color>
    </banned_colors>
    <!-- Players with the bypass permission colorizer.bypass will be able to bypass the restriction -->
    <!-- Kinda useless though, now that I look back on it -->
    <enable_bypass_permission>true</enable_bypass_permission>
    </ColorizeConfig>
commands:
    - name: /colorize [value]
      doc: 'Sets the caller''s chat color to [value]. Replace [value] with a hex or UnityEngine color code. Requires colorize.* or colorize.[value]'
    - name: /removecolor
      doc: 'Removes the caller''s custom chat color. Requires colorizer.remove.'

permissions:
    - name: colorize.*
      doc: 'Allows a player to set ANY color for his name.'
    - name: colorize.[value]
      doc: 'Allows a plyer to set a certain value as his color through /colorize. Can be hex or UnityEngine. REPLACE [value] WITH YOUR VALUE!'
    - name: colorize.remove
      doc: 'Allows a player remove his color through /removecolor.'
    - name: colorize.bypass
      doc: 'Allows a player to bypass the blacklist on colors.'
---
