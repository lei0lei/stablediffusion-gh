---
layout: default
title: Prompts
permalink: /prompts
has_children: true
has_toc: true
nav_order: 2
---
<details open markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
1. TOC
{:toc}
</details>

# prompts教程
常用prompts示例

## 相机视角


![]({{site.url}}/assets/images/prompts-camera.jpg)

## 图像质量
图像质量tags应该放在主体prompts的前面或者后面，默认情况下最好添加图像质量prompt，因为某些Lora会把 `masterpiece`,`best quality`之类的prompts作为出发提示词,具体使用什么图像质量tag还应该取决于基础模型，某些模型对特定的tag更加敏感，有一个经验是越动漫化的模型越需要这些tag。
### Quality Prompt

```
weird atmosphere, (best quality:1.1), (masterpiece:1.2), high quality shadow, beautiful detailed, (high detailed skin, skin details), (wide_landscape, 8k), beautiful face, detailed eyes, depth of field, dramatic light, best quality, highres, best shadow, best illumination,
```

### Negative Prompt

```
watermark, text, ((background characters)), realistic, (extra digits:1.4), (worst quality, low quality:1.4), (malformed hands:1.4), (poorly drawn hands:1.4), (mutated fingers:1.4), (extra limbs:1.35), (poorly drawn face:1.4), EasyNegative:1.2, bad-hands-5,
```
### LONG QUALITY:

``` 
extremely detailed CG unity 8k wallpaper, ultra-high-definition, (masterpiece:1.2), (best quality), (ultra-detailed), highres, sharp focus, clarity, fine textures, fine details, clear foreground, mid-ground, background elements, crisp edges, best illustration, an extremely delicate and beautiful, ultra-high color quality, high contrast**,** no watermark signature, painted by greg rutkowski makoto shinkai takashi takeuchi studio ghibli,
```

## 光照





## 风格




## 色彩




## 场景

对于 `scenes/setting/background`, 描述我们想要在一个场景中出现的内容，比如对于室内需要描述光源，有什么家具，地板墙壁的种类颜色等。
### Street

```
tokyo, city, street, building, lamppost, crosswalk,
```
### School 
```
classroom, window, chalkboard, chair, table,
```
### Gym
```
 gym, window, ceiling light, treadmill, elliptical trainer, dumbbells, barbells, exercise bike,
```
### Office
```
 office, office chair, table, paper, pen, window, ceiling light,
```
### Bar
```
 bar, ceiling light, counter, bar stool, wine, wine bottle, wine glass,
```
### Casino
```
casino, lobby, poker table, chair, cards, poker chip,
```

### Living Room
```
living room, couch, shelf, cabinet, ceiling light,
```

### Gaming Setup
```
gamer, table, gaming chair, computer, monitor, keyboard, mouse,
```

## 角色特征
### 通用角色特征
```
1girl/1boy
```
### 发型
```
length hair, color hair,
```
```
ponytail, twintail, braid, updo, etc.
```
```
color eyes,
```
```
heterochromia, fox eyes, etc.
```
```
breasts size
Large, medium, small, etc.
```
其他tags：
```
beautiful, cute, evil, naughty, short, tall, mature, skin tone, busty, slim, fit, muscular
```
比如:
```
1girl, long hair, orange hair, ponytail, green eyes, large breasts,
```


### 着装

这类prompts用来描述角色的穿着，如果我们添加了一个boots tag，最终的生成结果就会生成一个穿着boots的角色。


上身: 
```
shirts, blouses, sweaters, and jackets.
```
下身:

```
pants, shorts, skirts, and leggings, fall under this category.
```
鞋子
```
shoes, boots, sandals, and other types of footwear designed to protect and support the feet.
```

内衣
```
Clothing worn under other garments to protect, support, or cover intimate body parts, such as bras, panties, and undershirts.
```
Accessories
```
hats, scarves, belts, gloves, and jewelry that are worn to complement an outfit or provide additional functionality.
```
如果不使用outfit tag的话，最终生成的outfit会取决于正在用的模型。
prompt使用的时候从外到内,从上到下描述。

**Casual**
```
baseball cap, leather jacket, turtleneck, necklace, pleated skirt, thighhighs, garter straps,
```
**Student**
```
school uniform, gakuran, white shirt, serafuku, armband, plaid skirt, watch,
```
**Teacher**
```
teacher, long sleeves, button down polo, shirt tucked in, pencil skirt, thighhighs, garter straps,
```
**Gym**
```
ponytail, hair scrunchie, criss-cross halter, sports bra, athletic shorts / leggings, sweat,
```
**Sports (tennis/golf)**
```
visor cap, polo shirt, shirt tucked in, plaid skirt,
```
**Dress**
```
collarbone, bare shoulders, hair ornament, jewelry, choker, black dress, criss-cross halterneck, gloves,
```
**Suit (Formal)**
```
tuxedo, trousers, formal
```
**Suit (Business)**
```
business suit, blazer, white shirt, necktie, pants,
```
**Bunny Suit**
```
playboy bunny, rabbit ears, fake animal ears, collar, bowtie, wrist cuffs, navel, rabbit tail, thighhighs,
```
**Swimwear**
```
criss-cross bikini, sarong,bikini
```
**Military**
```
1. military, military uniform, peaked cap, coat, shirt, necktie, gloves, pants,
2. military, military uniform, It consists of a navy blue double-breasted tailcoat with standing collar faced white with gold edging worn with gold shoulder boards and gold laced blue trousers,
```
**Police**
```
police, police uniform, peaked cap, blue shirt, breast pocket, necktie, armband, gloves, blue pencil skirt, holster,
```


### 动作

准确描述正在发生的事情比如角色正在看向哪里，角色坐着还是站着(standing/sitting),手里是否拿着(holding)东西,正在做什么，摆的什么突出(striking)姿势.


----

## 负面prompts

A small archive of different negative prompt

**STANDARD NEGATIVE:** 
```
(worst quality, low quality:1.4), monochrome, zombie, (interlocked fingers),
```

**WITH NEGATIVE EMBEDDINGS:** 
```
(bad-hands-5:0.8), EasyNegative, ng_deepnegative_v1_75t,
```
**OTHER NEG EMBEDDINGS:**
```
bad_prompt_version2, badv3, (by bad-artist-anime), (by bad-artist-anime:0.8),
```

# Tips

## 括号使用

### `()`

### `[]`

### `{}`


### 权重


### 分区


### 分层