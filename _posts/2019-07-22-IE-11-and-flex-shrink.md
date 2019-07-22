---
layout: post
title: "IE 11 and issue with broken images inside flexbox."
date: 2019-07-21
subtitle: "IE 11 messes up flexbox and image children, due to bad defaults for flex-shrink."
tags: [Drupal, IE, CSS, Browser Compatiblity, Web Development, Frontend]
comments: true
---

IE 11 has a very wierd way of imposing flex-shrink on image children inside flexbox.

Even in 2019, [IE 11 only provides partial](https://caniuse.com/#feat=flexbox) supports for flexbox. Looks like Microsoft doesnt want to add new features in IE anymore and working full time on Edge, IE only gets security fixes now. This is very intresting considering IE is still default for older Windows OS and still used by a considerable chunk of traffic.

## Problem

If you have a flexbox div which contains a image. The Image gets stretched.

## Solution

Adding `flex-shrink: 0` for img tag fixes the issue.

## Reason

`flex-shrink` controls how an item inside flexbox will shrink, relative to the same flexbox container. IE has some very wierd way of handling defaults for this property, especially for images. Setting flex shrink to 0 fixes this issue for IE11.
