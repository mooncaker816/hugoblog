+++
title = "GCM"
date = 2018-08-26T19:17:56+08:00
draft = false

# Tags and categories
# For example, use `tags = []` for no tags, or the form `tags = ["A Tag", "Another Tag"]` for one or more tags.
tags = []
categories = []

# Featured image
# Place your image in the `static/img/` folder and reference its filename below, e.g. `image = "example.jpg"`.
# Use `caption` to display an image caption.
#   Markdown linking is allowed, e.g. `caption = "[Image credit](http://example.org)"`.
# Set `preview` to `false` to disable the thumbnail in listings.
[header]
image = ""
caption = ""
preview = true

+++

<!--more-->

# 1. GCM 认证加密

　　GCM 可以看成是 CTR 模式的升级版，在完成数据加密的前提下，同时完成数据的完整性验证。GCM 固定分组大小为 128bits，用于数据完整性验证的 MAC 称之为 GMAC。加密和 GMAC 计算使用同一秘钥。

# 2. GF
