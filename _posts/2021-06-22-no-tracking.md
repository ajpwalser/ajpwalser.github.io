---
layout: post
title: "This is a really, really, really long title"
tags: Admin
date: 2021-06-22
---

My privacy policy is simple: I don't track you.

No user data is collected or retained. There aren't any analytics, third-party scripts, or CDNs running on this website and no cookies are placed on your device. You also won't find any ads or paywalls.

I respect your privacy and encourage you to verify this using a browser extension like [UBlock Origin](https://ublockorigin.com/) or [Privacy Badger](https://privacybadger.org/). You can also review the full source code at my [GitHub repository](https://github.com/ajpwalser/ajpwalser.github.io).

I use <a href="https://buttondown.email/">Buttondown</a> for my newsletter and have opted out of analytics. This means Buttondown won't do things like track who opens, clicks, or forwards my emails.

{% if page.applause_button %}
  <applause-button class="mb6"
    color={{ site.accent_color | default:'rgb(79,177,186)' }}
    url={{ post.url | absolute_url }} >
  </applause-button>
  {% endif %}
