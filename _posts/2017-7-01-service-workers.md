---
layout: post
title: Service Worker
description: Making your site work offline.
image: ../../../../assets/images/sw-thumbnail.jpg
categories: Experiment Tools
---

What is a service worker?

A service worker is a script that your browser runs in the background, separate from a web page, opening the door to features that don't need a web page or user interaction. Today, they already include features like push notifications and background sync. In the future, service workers will support other things like periodic sync or geofencing. The core feature discussed in this tutorial is the ability to intercept and handle network requests, including programmatically managing a cache of responses. The reason this is such an exciting API is that it allows you to support offline experiences, giving developers complete control over the experience.

Below is an overly simplified version of the service worker lifecycle on its first installation:

<img src="../../../../assets/images/sw-lifecycle-thumbnail.jpg">

My website <a href="https://marcreyes.ph">homepage</a> now has a service worker. A snackbar notification will indicate whether or not the site caching was successfully achieved. Normally, service workers don't work on webpages that are not served over https so the secure homepage site is an advantage. Caching usually takes around 5-10 seconds to finish depending on the speed of your connection. Once done, turn off your internet connection and check whether the site still loads. Below is a sample of working and properly loaded portfolio content:

<img src="../../../../assets/images/sw-working-thumbnail.jpg">

You may also have the option to save it on your phone home screen like a native app. Yes, it works! Service workers will be added to all marcreyes.ph webpages, soon. <strong>Read more about service workers on the <a href="https://developers.google.com/web/fundamentals/getting-started/primers/service-workers">Google Developers</a> page.</strong>