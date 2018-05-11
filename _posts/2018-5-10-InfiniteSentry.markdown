---
layout: post
title: InfiniteSentry
description: 'InfiniteSentry allows sentries to fire infinitely. Infinite sentries are toggleable.'
download: 'https://github.com/IcePlugins/InfiniteSentry/releases'
github: 'https://github.com/IcePlugins/InfiniteSentry/'
documentation_block: |
  <?xml version="1.0" encoding="utf-8"?>
  <InfiniteSentryConfiguration xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <!-- If all sentries should be infinite or not. Disables sentry toggling. -->
    <allSentriesInfinite>true</allSentriesInfinite>
    <!-- Ignore this. It is used to store infinite sentries. -->
    <sentries />
  </InfiniteSentryConfiguration>
commands:
    - name: /toggleinfinite
      doc: 'Toggles infinite mode on the sentry that the player is looking at. Requires infinitesentry.toggle.'

permissions:
    - name: infinitesentry.toggle
      doc: 'Gives access to /toggleinfinite.'
---
