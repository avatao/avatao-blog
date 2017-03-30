---
layout: post
title: avatao XMaSS challenge
author: gabor
author_name: "Gabor Pek"
author_web: "https://www.crysys.hu/~pek"
---

[In our previous blog](https://blog.avatao.com/Your-first-avatao-Tuesday/), we gave you a small introduction to Cross-site Scripting (XSS) attacks and added some easy challenges to try your skills. It seems, however, that XSS is still one of the top vulnerabilites on the web, so we grasped the opportunity to prepare another small gift for you. 

<!--excerpt-->

This year was really interesting in terms of real use-cases. [One of the most recent findings was reported by (Dec 8, 2016) JP](https://klikki.fi/adv/yahoo2.html) about a stored XSS vulnerability in Yahoo Mail. According to JP's blog "The flaw was reported to Yahoo Security via [HackerOne](https://hackerone.com/yahoo) on November 12 and fixed on November 29, 2016. Yahoo awarded a bounty of $10,000 for the finding." In short, an attacker could perform a DOM-based XSS attack via dynamically generated HTML markups controlled by user-supplied values that were not properly sanitized.

Another interesting issue was when the AngularJS team decided to [remove their "expression sandbox" from AngularJS 1](https://docs.angularjs.org/guide/security) after [reporting escapes for all AngularJS 1 versions](https://www.youtube.com/watch?v=67Yc8_Bszlk&index=1&list=PLhixgUqwRTjwJTIkNopKuGLk3Pm9Ri1sF). It's important to emphasize that this sandbox was never intended to provide real protection against XSS attacks. It rather misled developers who kept relying upon it as a security feature.  

There are other XSS mitigation techniques such as [Javascript function overrides](https://www.trustwave.com/Resources/SpiderLabs-Blog/Detecting-Successful-XSS-Testing-with-JS-Overrides/), but these also failed to provide long-term XSS protection. A [recent blog entry on brutelogic.com](http://brutelogic.com.br/blog/bypassing-javascript-overrides/) suggests to use iframes to bypass the protection provided by "js-override.js".

After this small update on recent XSS techniques, you can try your skills again by solving our [XmaSS challenge](https://platform.avatao.com/paths/2bf3c9cb-f759-4915-9a2f-f30164c45fce/challenges/f4d9b9a0-42a7-11e6-bdf4-0800200c9a66). Enjoy it!

If you like our posts and challenges, please follow us on [twitter](https://twitter.com/theavatao) and [facebook](https://www.facebook.com/theavatao/). 


We wish you a happy Christmas!
