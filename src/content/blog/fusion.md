---
author: Jay
pubDatetime: 2024-05-12T15:22:00Z
modDatetime: 2024-05-12T15:22:00Z
title: Homeassistant平板主题分享《ha-fusion》
slug: hafusion
featured: false
draft: false
tags:
  - homeassistant
description:
  一款设计非常好看的HA平板主题《ha-fusion》，现代感、美观，很合适智能家居上墙。
---



## ha-fusion

最近发现一款设计非常好看的HA平板主题《ha-fusion》，现代感、美观，很合适智能家居上墙。
官方地址：https://github.com/matt8707/ha-fusion

我根据自己的使用习惯搭建了下面的布局，喜欢的可以复制代码自己修改。

![fusion](@assets/images/hafusion.png)

> 代码

```
  views:
    - name: 全屋
      id: 9785970305331
      sections:
        - type: horizontal-stack
          sections:
            - name: Person
              items:
                - id: 2173327509169
                  type: button
                  entity_id: device_tracker.jayzi
                  icon: https://s2.loli.net/2024/03/10/a43ARiIOTr2kbqe.jpg
                - id: 3883267301497
                  type: button
                  entity_id: device_tracker.shelley_iphone
                  icon: https://s2.loli.net/2024/03/10/FKvA2U9DH1VLTMa.jpg
              id: 2797348998224
            - name: 场景
              items:
                - id: 7642811242324
                  type: button
                  entity_id: scene.shui_mian_mo_shi
                - id: 7398469928938
                  type: button
                  entity_id: scene.hui_jia_mo_shi
                - id: 5489388662670
                  type: button
                  entity_id: scene.chi_jia_mo_shi
              id: 5060684822052
            - name: ''
              items:
                - id: 8418972523762
                  type: button
                  entity_id: scene.you_xi_yu_le
                - id: 7339959590536
                  type: button
                  entity_id: scene.yue_du_mo_shi
                - id: 3050487022681
                  type: button
                  entity_id: scene.guan_ying_mo_shi
              id: 3223702350741
          id: 9102765011749
        - name: 空调新风
          items:
            - id: 2502702309003
              type: button
              entity_id: climate.thermostat_1
            - id: 7125855355793
              type: button
              entity_id: climate.thermostat_2
            - id: 3492385574677
              type: button
              entity_id: climate.thermostat_4
            - id: 8596654288268
              type: button
              entity_id: climate.thermostat_3
            - id: 9061592763266
              type: button
              entity_id: fan.magic_switch_s1e_e67a_switch_1
              name: 新风小
            - id: 5450980421245
              type: button
              entity_id: fan.magic_switch_s1e_e67a_switch_2
              name: 新风大
          id: 5781123198581
      icon: fluent:home-more-24-filled
    - name: 客厅
      id: 7006312930170
      sections:
        - name: 灯
          items:
            - id: 1171957582504
              type: button
              entity_id: light.yeelink_ceiling19_ff5d_light
            - id: 8040094971718
              type: button
              entity_id: light.yp3_194779_light
            - id: 4132637797757
              type: button
              entity_id: light.yp3_2037724_light
            - id: 5168738346985
              type: button
              entity_id: light.yp3_192538_light
            - id: 4359537545174
              type: button
              entity_id: light.yp3_2069203_light
            - id: 5188334199071
              type: button
              entity_id: light.yp3_192540_light
            - id: 4911079142829
              type: button
              entity_id: light.shhf_slwfc3_6ae4_light
            - id: 7380002196489
              type: button
              entity_id: light.yp3_2039148_light
          id: 4197812188027
        - name: 玄关
          items:
            - id: 3758064626884
              type: button
              entity_id: light.yp3_2037779_light
            - id: 2613750003382
              type: button
              entity_id: light.yp3_2118133_light
          id: 7896665053360
        - name: 窗帘
          items:
            - id: 687807543730
              type: button
              entity_id: cover.ke_ting_chuang_lian
            - id: 5193477917940
              type: button
              entity_id: cover.curtain_5
            - id: 6153011627580
              type: button
              entity_id: cover.curtain_6
          id: 3130879758314
      icon: ion:tv-sharp
    - name: 主卧
      id: 6935703711047
      sections:
        - name: 灯
          items:
            - id: 9105014448875
              type: button
              entity_id: light.yp3_192552_light
            - id: 271813793020
              type: button
              entity_id: light.yp3_2038926_light
            - id: 6460823549957
              type: button
              entity_id: light.yp3_2037859_light
            - id: 1590908307070
              type: button
              entity_id: light.yeelink_ceiling20_8f86_light
          id: 7597341702355
        - name: 窗帘
          items:
            - id: 3520189732653
              type: button
              entity_id: cover.zhu_wo_chuang_lian
            - id: 1834210718488
              type: button
              entity_id: cover.curtain
            - id: 2747498518799
              type: button
              entity_id: cover.curtain_2
          id: 4480412490226
      icon: cbi:roomsbedroom
    - name: 次卧
      id: 1561391928976
      sections:
        - name: 灯
          items:
            - id: 3109564236231
              type: button
              entity_id: light.yp3_2069121_light
            - id: 2873917323186
              type: button
              entity_id: light.yp3_2037767_light
            - id: 9035695400174
              type: button
              entity_id: light.yp3_2039046_light
            - id: 4355935498262
              type: button
              entity_id: light.yeelink_ceiling13_a483_light
          id: 46539145302
        - name: 窗帘
          items:
            - id: 9752044484880
              type: button
              entity_id: cover.ci_wo_chuang_lian
            - id: 451828339452
              type: button
              entity_id: cover.curtain_3
            - id: 4018611886663
              type: button
              entity_id: cover.curtain_4
          id: 8684932901314
      icon: bxs:baby-carriage
    - name: 书房
      id: 7611389428356
      sections:
        - name: 灯
          items:
            - id: 8181819316293
              type: button
              entity_id: light.yeelink_ceiling20_dd55_light
            - id: 9499348203576
              type: button
              entity_id: light.yp3_2037881_light
            - id: 5406021467277
              type: button
              entity_id: light.xiang_xun_deng_switch
          id: 5108400846558
        - name: 窗帘
          items:
            - id: 7552370827435
              type: button
              entity_id: cover.shu_fang_chuang_lian
            - id: 9924964450341
              type: button
              entity_id: cover.68abbc18f4cb_motor
            - id: 5211477540946
              type: button
              entity_id: cover.ccb5d1a46a2a_motor
          id: 1755556017345
      icon: streamline:computer-pc-desktop-solid
    - name: 厨房
      id: 6422525877707
      sections:
        - name: 灯
          items:
            - id: 7006550199376
              type: button
              entity_id: light.aqara_single_wall_switch_h1_switch
          id: 1114309556053
      icon: material-symbols:kitchen
    - name: 阳台
      id: 1496173915784
      sections:
        - name: ''
          items:
            - id: 9535812987599
              type: button
              entity_id: cover.mrbond_m33a_39c8_airer
              name: 晾衣架
            - id: 1980937601441
              type: button
              entity_id: light.mrbond_m33a_39c8_light
          id: 9710084170548
      icon: material-symbols:balcony
    - name: 耗材
      id: 2216747344892
      sections:
        - name: 耗材
          items:
            - id: 8975460358721
              type: button
              entity_id: sensor.48574300e09b_battery
            - id: 5252750592171
              type: button
              entity_id: sensor.68abbc18f4cb_battery
            - id: 4115569849074
              type: button
              entity_id: sensor.ccb5d1a46a2a_battery
            - id: 9446829336364
              type: button
              entity_id: sensor.0x54ef441000b062a3_battery
              name: 高精度传感器厨房
            - id: 6417565677743
              type: button
              entity_id: sensor.0x54ef441000b066c8_battery
              name: 高精度传感器主卫
            - id: 3159904964681
              type: button
              entity_id: sensor.68abbc198d0f_battery
          id: 3368840332146
  sidebar:
    - id: 5112809698209
      type: time
    - id: 2510798422269
      type: date
    - id: 4615656004910
      type: weather
      entity_id: weather.qingpu
      icon_pack: meteocons
      weather_sensor: sensor.openweathermap_forecast_temperature_low
      extra_sensor: sensor.openweathermap_humidity
    - id: 1220408126158
      type: template
      template: >-
        ❄️空调 {{ states.climate | selectattr('attributes.hvac_action', 'eq',
        'cooling') | list | length }} | {{ states.climate |
        selectattr('attributes.hvac_action', 'eq', 'heating') | list | length }}  
    - id: 4461293680900
      type: template
      template: >-
        💡灯 {{ expand('light.deng') | selectattr('state','eq','on') | list | count
        }}
    - id: 1470493485743
      type: graph
      entity_id: sensor.shineiwendu
    - id: 9848780913138
      type: bar
      entity_id: sensor.shi_nei_shi_du
      name: ''
    - id: 4619014749499
      type: graph
      entity_id: sensor.0x54ef4410006ca2ca_tvoc
      name: 空气质量
  theme: muted
  hide_views: false
  hide_sidebar: false
  sidebarWidth: 304

```
