---
layout: post
title: BoneHurtingBullets
description: 'Allow players to damage bones by shooting and hitting. Configurable chances.'
download: 'https://github.com/IcePlugins/BoneHurtingBullets/releases'
github: 'https://github.com/IcePlugins/BoneHurtingBullets/'
documentation_block: |
  <?xml version="1.0" encoding="utf-8"?>
  <BoneHurtingBulletsConfiguration xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <boneBreakingChances>
      <!-- One entity representing a chance for a player's bones to be broken on damage to the limb -->
      <BulletLimbDamageChance>
        <!-- The limb in question. DO NOT CHANGE THESE. They are automatically generated. -->
        <Limb>LEFT_FOOT</Limb>
        <!-- The chance out of 100 for a player's bones to break. Set it to 25, and they will break 25% of the time on hit. Whole numbers only. -->
        <BreakChance>25</BreakChance>
      </BulletLimbDamageChance>
      <BulletLimbDamageChance>
        <Limb>LEFT_LEG</Limb>
        <BreakChance>25</BreakChance>
      </BulletLimbDamageChance>
      <BulletLimbDamageChance>
        <Limb>RIGHT_FOOT</Limb>
        <BreakChance>25</BreakChance>
      </BulletLimbDamageChance>
      <BulletLimbDamageChance>
        <Limb>RIGHT_LEG</Limb>
        <BreakChance>25</BreakChance>
      </BulletLimbDamageChance>
      <BulletLimbDamageChance>
        <Limb>LEFT_HAND</Limb>
        <BreakChance>25</BreakChance>
      </BulletLimbDamageChance>
      <BulletLimbDamageChance>
        <Limb>LEFT_ARM</Limb>
        <BreakChance>25</BreakChance>
      </BulletLimbDamageChance>
      <BulletLimbDamageChance>
        <Limb>RIGHT_HAND</Limb>
        <BreakChance>25</BreakChance>
      </BulletLimbDamageChance>
      <BulletLimbDamageChance>
        <Limb>RIGHT_ARM</Limb>
        <BreakChance>25</BreakChance>
      </BulletLimbDamageChance>
      <BulletLimbDamageChance>
        <Limb>LEFT_BACK</Limb>
        <BreakChance>25</BreakChance>
      </BulletLimbDamageChance>
      <BulletLimbDamageChance>
        <Limb>RIGHT_BACK</Limb>
        <BreakChance>25</BreakChance>
      </BulletLimbDamageChance>
      <BulletLimbDamageChance>
        <Limb>LEFT_FRONT</Limb>
        <BreakChance>25</BreakChance>
      </BulletLimbDamageChance>
      <BulletLimbDamageChance>
        <Limb>RIGHT_FRONT</Limb>
        <BreakChance>25</BreakChance>
      </BulletLimbDamageChance>
      <BulletLimbDamageChance>
        <Limb>SPINE</Limb>
        <BreakChance>25</BreakChance>
      </BulletLimbDamageChance>
      <BulletLimbDamageChance>
        <Limb>SKULL</Limb>
        <BreakChance>25</BreakChance>
      </BulletLimbDamageChance>
    </boneBreakingChances>
  </BoneHurtingBulletsConfiguration>
---
