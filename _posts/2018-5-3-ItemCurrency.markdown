---
layout: post
title: ItemCurrency
description: 'Allows you to use items as currency in the buying/selling of goods.'
download: 'https://github.com/IcePlugins/ItemCurrency/releases'
github: 'https://github.com/IcePlugins/ItemCurrency/'
documentation_block: |
  <?xml version="1.0" encoding="utf-8"?>
  <ItemCurrencyConfiguration xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <Money>
      <!-- One money element. Id is the ID of the item, value is how much value that item holds. If I have 3 berries in my inventory and they are configured to value 5, then I would have $15. -->
      <MoneyValue Id="1051" Value="5" />
      <MoneyValue Id="1052" Value="10" />
      <MoneyValue Id="1053" Value="20" />
      <MoneyValue Id="1054" Value="50" />
      <MoneyValue Id="1055" Value="100" />
      <MoneyValue Id="1056" Value="1" />
      <MoneyValue Id="1057" Value="2" />
    </Money>
    <Prices>
      <!-- One item element. 'Id' is the ID of the item; 'Name' is just an identifier for easier configuration and can be ignored; 'BuyPrice' is the buy price; 'SellPrice' is the sell price. You can set the price to 0 to disable buying/selling. -->
      <ItemPrice Id="2" Name="Work Jeans" BuyPrice="10" SellPrice="5" />
      <ItemPrice Id="3" Name="Orange Hoodie" BuyPrice="0" SellPrice="0" />
      <ItemPrice Id="4" Name="Eaglefire" BuyPrice="0" SellPrice="0" />

      <!-- For the sake of simplicity, this list has been truncated. All Unturned item IDs generated on plugin start so that you don't have to manually input IDs. -->

    </Prices>
    <!-- What currency symbol the plugin will display. -->
    <CurrencySymbol>$</CurrencySymbol>
  </ItemCurrencyConfiguration>
commands:
    - name: /buy [id/name] [amt]
      doc: 'Lets a player buy items that are registered for sale. [amt] is an optional parameter, it will default to 1.'
    - name: /sell [id/name] [amt]
      doc: 'Lets a player sell items that are registered for sale. [amt] is an optional parameter, it will default to 1.'
    - name: /balance
      doc: 'Displays the cumulative value of all the cash items in the player''s inventory.'
    - name: /value [id/name]
      doc: 'Displays the value of a certain item.'

permissions:
    - name: itemcurrency.buy
      doc: 'Allows a player to use /buy'
    - name: itemcurrency.sell
      doc: 'Allows a player to use /sell'
    - name: itemcurrency.value
      doc: 'Allows a player to use /value'
    - name: itemcurrency.balance
      doc: 'Allows a player to use /balance'
---
Uconomy compatibility layer coming soon...