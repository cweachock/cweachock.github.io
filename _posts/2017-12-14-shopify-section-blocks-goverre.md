---
layout: post
title: Using Section Blocks for Inventory Listing 
summary: How to use Shopify's section blocks to create a private inventory listing page for sales reps
category: articles
tags: shopify
date: 2017-12-14
---

A while ago the [Founders](https://goverre.com/pages/our-story) of [Goverre](https://goverre.com/pages/about): a modern re-sealable to-go cup used for wine reached out to me to help them design a landing page where their sales reps could easily see what products they had in stock. 

![Goverre Inventory Section Listing Block](/images/Goverre--Custom-Invetory-Listing-Page-Screenshot-Using-Shopify-Section-Blocks.png)

They wanted something that was easily editable from the [Shopify](https://www.shopify.com/?ref=chris-weachock-design) admin to show product pictures, select and show product availability, and indicate the title/UPC value. In addition, they wanted it to be password protected. 

Turns out Shopify has an excellent tool with their new sections called “[section blocks](https://www.shopify.com/partners/blog/shopify-section-block)”. Using section blocks, you can easily loop a set attributes and different offers set using the schema. 

Using Shopify’s liquid editor, I first created a section called inventory-listing.liquid (or whatever you want to call it). The template and CSS grids are handled
with the free [Boundless theme](https://themes.shopify.com/themes/boundless/styles/vibrant) designed and developed by [Shopify](https://www.shopify.com/?ref=chris-weachock-design). And the page is protected by the app [Locksmith](https://apps.shopify.com/locksmith). Which turned out to accomplish the job quite well. 

Elements I added to edit are title, sub title, product title, product image, and availability. 

Here’s the markup for html: 

{% gist d13f5f2c15efe5e39d166995a60d0522 %}



