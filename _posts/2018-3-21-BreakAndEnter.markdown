---
layout: post
title: BreakAndEnter
description: 'Admin utility to access locked storage containers, force doors open, and destroy barricades/structures.'
download: 'https://github.com/IcePlugins/BreakAndEnter/releases'
github: 'https://github.com/IcePlugins/BreakAndEnter/'
documentation_block: |
  <?xml version="1.0" encoding="utf-8"?>
  <BreakAndEnterConfiguration xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" />
commands:
    - name: /storage
      doc: 'Gives a player access to the storage unit that they are looking at. Requires breakandenter.storage.'
    - name: /door
      doc: 'Toggles the door''s open/closed state that the player is looking at. Requires breakandenter.door.'
    - name: /destroy
      doc: 'Destroys a structure or barricade that the player is looking at. Requires breakandenter.destroy.'

permissions:
    - name: breakandenter.storage
      doc: 'Gives a player access to /storage'
    - name: breakandenter.door
      doc: 'Gives a player access to /door'
    - name: breakandenter.destroy
      doc: 'Gives a player access to /destroy'
---
