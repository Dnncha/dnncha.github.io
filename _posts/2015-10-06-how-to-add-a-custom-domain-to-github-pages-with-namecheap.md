---
layout: post
title: "How to add a custom domain to GitHub Pages with Namecheap"
date: 2015-10-06 19:31:36
image: '/assets/img/'
description: "I've written up the steps for Namecheap users, in case you've found yourself scratching your head at the new DNS configuation page. "
tags: 
- github pages
- jekyll
- namecheap
categories:
twitter_text: 'How to add a custom domain to Github Pages with Namecheap'
---

Once you've bought your domain, log in to your Namecheap dashboard, where you'll find a list of all your domains. Click  **manage** on the domain you're assigning to GithubPages, and then click the **Advanced DNS** tab.

Now click on *Manage* your *Host Records* to add some DNS records.

We're going to add two A records, with *Host* set to @. The first one should point at **192.30.252.153**, and the second A record should point to **192.30.252.154**

Next, we'll add a CNAME record, with **Host** set to **yoursite.github.io**

After that, you'll want to switch off the preexisting URL Record, with the type *URL redirect*. If you don't switch this off, you may find that Chrome throws a *Too many redirects* error, whereas Safari doesn't seem to care.

Enjoy, and please do me know how you get on!






