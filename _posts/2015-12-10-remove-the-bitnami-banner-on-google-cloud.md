---
layout: post
title: "How to remove the Bitnami banner on WordPress on Google Cloud"
date: 2015-12-10 10:31:36
image: '/assets/img/'
description: "Removing that banner is easy, but not perfectly documented. "
tags: 
- google cloud
- wordpress
- bitnami
categories:
twitter_text: 'How to remove the Bitnami banner on WordPress on Google Cloud.'
---

So you jump on the Google Cloud Wordpress bandwagon for extra speed, security etc, and you opt for the simple one-click-install of Wordpress from Bitnami. Everything works great except for a big stupid banner that sits at the bottom of your site all day. 

If you look up the Bitnami documentation, they tell you to run `/opt/bitnami/apps/wordpress/bnconfig --disable_banner 1` but your Google cloud instance won't give you permission to run that. 

There's a simple solution that'll surely cause you to Picard facepalm. First run the `sudo su` command to become the superuser. Then run `/opt/bitnami/apps/wordpress/bnconfig --disable_banner 1` again. It returns no output, but if you refresh you'll find that pesky banner has disappeared forever. Hallelujah. 






