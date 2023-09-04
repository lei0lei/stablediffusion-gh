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
人物常用prompts示例

## 相机视角

![]({{site.url}}/assets/images/prompts-camera.jpg)


## 图像质量
图像质量tags应该放在主体prompts的前面或者后面，默认情况下最好添加图像质量prompt，并且某些Lora会把 `masterpiece`,`best quality`之类的prompts作为出发提示词。
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

### 发型



### 着装




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