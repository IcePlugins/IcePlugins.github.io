---
layout: post
title: BigSentry
description: 'Turns your small sentry into the BIG sentry. Configurable sentry slot extender that works with all sentries.'
download: 'https://github.com/IcePlugins/BigSentry/releases'
github: 'https://github.com/IcePlugins/BigSentry/'
documentation_block: |
  <?xml version="1.0" encoding="utf-8"?>
  <BigSentryConfiguration xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <!-- Global width (x) override for all sentries -->
    <globalWidthOverride>8</globalWidthOverride>
    <!-- Global height (y) override for all sentries -->
    <globalHeightOverride>8</globalHeightOverride>

    <!-- Ids that the plugin will ignore -->
    <ignoreIds>
      <!-- Id that the plugin will ignore -->
      <Id>1372</Id>
    </ignoreIds>

    <!-- Overrides for default global sizes -->
    <overridesById>
      <!-- One override group, copypaste to make more -->
      <Sentry>
        <!-- Id of the sentry that it will override -->
        <Id>1373</Id>
        <!-- Width override -->
        <Width>6</Width>
        <!-- Height override -->
        <Height>3</Height>
      </Sentry>
    </overridesById>
  </BigSentryConfiguration>
---
