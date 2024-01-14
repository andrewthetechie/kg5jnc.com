---
title: Cats
subtitle: Communication and Telemetry System - A Modern APRS Replacement
date: 2024-01-12T17:12:49-06:00
slug: eab4d80
description:
keywords:
  - packet
  - cats
  - digital
  - aprs
  - uhf
license:
comment: false
weight: 0
tags:
  - packet
  - uhf
  - 70cm
  - digital
categories:
  - uhf
  - digital
  - packet
hiddenFromHomePage: false
hiddenFromSearch: false
hiddenFromRss: false
hiddenFromRelated: false
summary:
toc: true
math: false
lightgallery: false
password:
message:
repost:
  enable: false
  url:
# See details front matter: https://fixit.lruihao.cn/documentation/content-management/introduction/#front-matter
---

I recently learned about [CATS](https://www.zeroretries.org/p/zero-retries-0129#%C2%A7communication-and-telemetry-system-cats-rethinking-aprs-paradigms) from the excellent [Zero Retries by Steve Stroh](https://www.zeroretries.org/p/zero-retries-0129#%C2%A7communication-and-telemetry-system-cats-rethinking-aprs-paradigms) (you should subscribe, its an excellent newsletter). To quote from the CATS documentation:

> At its core, CATS is a packet radio standard primarily designed for autonomous position reports, but is versatile enough to support a much wider scope of communication. CATS packets are extremely versatile, consisting of multiple "Whiskers" which make up the packet. Whiskers come in several types. For example, a typical CATS position beacon would likely contain an Identification Whisker, GPS Whisker, and potentially a Comment Whisker and Timestamp Whisker. Different Whiskers can be mixed and matched to allow a wide range of data to be encoded. Detailed information on CATS can be found in the standard, linked below.

Stephen's goal is to build a modern replacement for APRS with quite a few improvements. CATS uses FSK rather than FM, has a faster data rate (9600baud), and has forward error correction. CATS uses 70cm rather than the 2m that is more common with APRS.

The project is still work-in-progress, but there has been tremendeous progress already. There is a [well-documented standard](https://gitlab.scd31.com/cats/cats-standard), [reference](https://gitlab.scd31.com/cats/ham-cats) [implementations](https://gitlab.scd31.com/cats/felinet-server) [written](https://gitlab.scd31.com/cats/felinet-aprs-relay) in rust, and a design for a [standalone transciever](https://gitlab.scd31.com/cats/mobile-transceiver). The rust implementation is interesting to me as it is [easy to use rust projects](https://pyo3.rs/v0.20.2/) in python (my preferred language).

I'm not currently running any CATS at my shack, but will be watching the project. The cat puns alone are enough to keep my interest!

<!--more-->
