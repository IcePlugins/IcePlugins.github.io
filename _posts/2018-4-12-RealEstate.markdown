---
layout: post
title: RealEstate
description: 'Rewrite of the abandoned HousePlugin with less lag. Allows players to buy pre-existing in-game houses.'
download: 'https://github.com/IcePlugins/RealEstate/releases'
github: 'https://github.com/IcePlugins/RealEstate/'
documentation_block: |
  <?xml version="1.0" encoding="utf-8"?>
  <RealEstateConfiguration xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <!-- Currency symbol used in RealEstate chat messages -->
    <currencySymbol>$</currencySymbol>
    <!-- Default max homes for people who don't have realestate.maxhouses.[number] -->
    <defaultMaxHomes>1</defaultMaxHomes>
    <!-- How often the plugin should check for and collect house payments in seconds. You can change this to a smaller or larger value if you'd like. -->
    <paymentCheckIntervalInSeconds>10</paymentCheckIntervalInSeconds>
    <!-- How often a player will pay the upkeep for their house in minutes. The money paid is the price of the house. IF YOU WANT TO DISABLE THIS, SET IT TO 0. -->
    <feePaymentTimeInMinutes>1440</feePaymentTimeInMinutes>
    <!-- If structures inside a home should be destroyed on an eviction. -->
    <destroyStructuresOnEviction>false</destroyStructuresOnEviction>

    <!-- Ignore everything below this, it's used for data storage. -->
    <homes />
    <displayNames />
  </RealEstateConfiguration>
commands:
    - name: /abandonhouse
      doc: 'Lets a player abandon the house that they are standing in. Requires the player to actually own the house. Permission: realestate.abandonhouse'
    - name: /addhouse
      doc: 'Lets a player add the house that they are standing in to the catalog so that other players can buy it. Should be admin only. Permission: realestate.addhouse'

    - name: /buyhouse
      doc: 'Lets a player buy the house that they are standing in. The house must be in the catalog. Permission: realestate.buyhouse'

    - name: /checkhouse
      doc: 'Lets the player check the price and owner of the house that they are standing in. The house must be in the catalog. Permission: realestate.checkhouse'

    - name: /evicthouse
      doc: 'Evicts the owner of the house that the player is standing in. Should be admin only. Permission: realestate.evicthouse'

    - name: /removehouse
      doc: 'Removes the house that the player is standing in from the catalog. Should be admin only. Permission: realestate.removehouse'

permissions:
    - name: realestate.maxhouses.[number]
      doc: 'Sets the maximum number of houses for the permission holder. Repace [number] with a number.'
    - name: realestate.abandonhouse
      doc: 'Gives access to /abandonhouse.'
    - name: realestate.addhouse
      doc: 'Gives access to /addhouse. Should be admin only.'
    - name: realestate.buyhouse
      doc: 'Gives access to /buyhouse.'
    - name: realestate.checkhouse
      doc: 'Gives access to /checkhouse.'
    - name: realestate.evicthouse
      doc: 'Gives access to /evicthouse. Should be admin only.'
    - name: realestate.removehouse
      doc: 'Gives access to /removehouse. Should be admin only.'
---
REQUIRES UCONOMY. IF YOU WANT TO USE AVIECONOMY, USE THE UCONOMYTOAVI WRAPPER ON ROCKETHUB.
<br />
Plugin concept <a href="https://hub.rocketmod.net/product/houseplugin/">here</a>. This plugin was abandoned and broken and I was requested to fix it. It was a complete mess, so I just rewrote it.
