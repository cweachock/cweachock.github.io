---
layout: post
title: Case Study: How create a product for pre-ordering
summary: In this case study I breakdown how to modify Shopify's Brooklyn template to create a pre-order AJAX template   
category: articles
tags: shopify
date: 2018-02-20
---

## Overview

After a successful Indiegogo campaign—[Alexander Simone](http://www.alexandersimone.com/), founder of [Pronto Concepts](https://www.prontoconcepts.com) wanted to take pre-orders online before making his big debut on [ABC’s Shark Tank](http://abc.go.com/shows/shark-tank). He needed a functioning website that reflected his brand and offered the ability to capture emails, discounted pre-sales, offer packages, as well as handle the traffic that comes from the primetime spotlight. As a true ecommerce platform, [Shopify](https://www.shopify.com/?ref=chris-weachock-design&utm_content=psite&utm_medium=website&utm_source=chrisweachock.com) was the best solution for him, and hasn’t disappointed since. 

![Pronto Concepts](/case-studies/pronto-concepts/Case_Study_Pronto_Concepts_Introduction_Home.png)

From concept to creation, I helped the transition his site from Squarespace to a fully functioning Ecommerce pre-order store on [Shopify](https://www.shopify.com/?ref=chris-weachock-design&utm_content=psite&utm_medium=website&utm_source=chrisweachock.com). The timeline was about two weeks to make a website to take pre-sales, and collect customer and potential customer information. Custom product pages that were unique to his brand were created as well as dynamic sections and pre-ordering to allow easy purchase and buying power. 

### Context, Challenge, and Process

Most modern day shopping carts are dynamic. To start, I helped narrow down and choose a skeleton template that had a dynamic cart to build off of that brought together a mobile mindset then customized it collaboratively working with another developer refining user experience.. The challenge was to make something that wasn’t too complicated but functional and resonated well making the product the focal point. In this case, Shopify’s(https://www.shopify.com/?ref=chris-weachock-design&utm_content=psite&utm_medium=website&utm_source=chrisweachock.com) well designed [Brooklyn theme](https://themes.shopify.com/themes/brooklyn/styles/classic) provided much of the flexibility and mobile first mindset that allowed his product to shine much like a modern technology product would sell.

![Shopify Brooklyn Theme](/case-studies/pronto-concepts/Case_Study_Pronto_Concepts_Brooklyn_Theme_Foundation.png)
![Pronto Concepts Product Section](/case-studies/pronto-concepts/Case_Study_Pronto_Concepts_Home_Page_Product_Section.png)

#### The First Rough Pass or Sprint 1

I try to break down my phases of design and development into short bursts of work. This makes it more manageable for both the entrepreneur and myself (most of the time). Usually I open myself up to all pools of collaboration. Alexander conveniently set up a tasks list using Google Docs and email for much of our beginning work. This helped us streamline much of the changes and make quick work through the short iterations before Shark Tank.

![Google Spreadsheet for organization and collaboration](/case-studies/pronto-concepts/Pronto-Concepts-Google-Spreadsheet-Tasks-List.png) 

Tasks were separated between me, Alexander, and [Quan Tran](https://quan.github.io/): an additional developer on the project. I began much of the work populating the site transitioning web fonts, colors, aesthetic, and, helping set up basic settings. Groundwork for much of the site was set for the homepage, product page, and other landing pages. In addition to a custom [pre-order page](https://prontoconcepts.com/pages/pre-order).

#### Sprint 2: Pre-order development and product page design.  

After the first rough pass was done, product pages needed a different layout to dial in what the frontend of the website was to look like. Utilizing [Shopify’s](https://www.shopify.com/?ref=chris-weachock-design&utm_content=psite&utm_medium=website&utm_source=chrisweachock.com) section elements, a new product page was created based off of mockup design(s) created in Illustrator. 

![Google Spreadsheet for organization and collaboration](/case-studies/pronto-concepts/Case_Study_Pronto_Concepts_Pronto_Bev_Product_Page_Above_Fold.png) 

The product page was set up to emulate a modern technology product with a traditional product image on the left, and product description and text on the right. The ProntoBev was set with package variant options to allow customers to choose which “offer” they wanted. Originally the product offers were to be split out into different products for the Shark Tank specials. But for easier UX I suggested that they be combined into variant options. This allowed for easier selection and checkout flow.

![Google Spreadsheet for organization and collaboration](/case-studies/pronto-concepts/Case_Study_Pronto_Concepts_Pronto_Bev_Product_Page_Above_Fold_Variant_Selection.png) 


Much of the foundation for the product page was built with sections. These were then referenced in the theme.liquid file and dynamically shown with control flow tags. Each product ([The ProntoBev](https://prontoconcepts.com/products/prontobev-wine-chiller) and [ProntoAer](https://prontoconcepts.com/products/prontoaer-wine-aerator) had it’s own page redesign. So they had to be completely refactored. Initially I did a rough first pass then it was handed off. 

### Building out the Pre-order implementation section

Because the template already was built off of [Shopify’s Timber framework](https://shopify.github.io/Timber/), the site allowed for a [dynamic AJAX add to cart](https://help.shopify.com/themes/development/getting-started/using-ajax-api). When someone adds a product to their shopping cart, it triggers a drawer to open (from the side or wherever) so they can stay on the same page and continue shopping. This is where the structure of the product variants comes into play. 

![Google Spreadsheet for organization and collaboration](/case-studies/pronto-concepts/Case_Study_Pronto_Concepts_Pronto_Bev_Liquid_Sections_Screenshot.png) 


Originally, I created a page for the product variants using the site’s internal grid system and [cart.js](https://cartjs.org/). However, as issues presented themselves with promise chaining (something I don’t yet understand) and how actual orders were being received by Shopify and the place in which they were being ordered proved to be difficult. After doing some research, I built the function to pre-order using an onclick event which triggered an [AJAX call](https://help.shopify.com/themes/development/getting-started/using-ajax-api) to open a javascript popup indicating a product was added to the cart. 

![AJAX add to cart modal](/case-studies/Pronto-Concepts-Added-To-Cart-AJAX.png) 

### Small UX changes/modifications

Other things I modified or suggested was a sticky navigation that showed on scroll down in addition to hiding elements like the pre-order button on the actual page, and also changing the color of the checkout button, layout of the footer, adding the shopify badge, and lity.js a lightweight library that plays youtube videos in a popup on selection or click instead of loading the iframe directly into the page. 

Check out [the product](https://www.prontoconcepts.com) It's pretty cool!
