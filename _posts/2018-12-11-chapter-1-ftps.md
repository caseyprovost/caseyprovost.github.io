---
layout: post
title: "Chapter 1: FTPS & Ruby"
---

Before last month I had no idea that FTPS was a thing. Partly because a lot of FTP clients default between FTP and SFTP. Largely it is because it was referred to as FTP with ssl, FTP Secure, FTP-SSL, and other variants. It turns out that it is a common protocol when communicating with bank servers, who knew? Now I know what you are thinking...why is FTP interesting? The answer: mainly because Ruby JUST implemented support in Ruby 2.4!

If you have researched this topic or needed to implement FTPS in ruby yourself you are probably familiar with [Double Bag](https://github.com/bnix/double-bag-ftps). It was a great library and still is for those of you who have not moved to Ruby 2.4 and beyond...if you have though you were likely immediately depressed to find that Double Bag no longer worked for you. Sadly is it not compatible with 2.4. Don't lose hope though! After reading though the issues on Double Bag I found that other developers had discovered the new feature in 2.4 and had been able to move forward using that.

And just like that I was able to progress on my project as well..for a second. Then I discovered that there is VERY little documentation on the Ruby Net::FTP class with respect to SSL and certificate usage.
