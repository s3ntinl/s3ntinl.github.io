
---
title: "OSWP: Tips and Tricks to Pwn all Networks!"
summary: "I recently went through the OSWP certification, and in this post I’ll share how I prepared, what went wrong, and what I learned from the whole experience."
categories: ["Post","Blog",]
tags: ["certification experience"]
#externalUrl: ""
#showSummary: true
draft: false
date: 2025-11-01

---

## **I Passed the OSWP!**

I'm proud to annouce that I've achieved the **Offensive Wireless Professional (OSWP)** certification. This certification grants great complementary knowledge to OSCP, making you a better Penetration Tester. Don't forget Wi-Fi Networks are everywhere, and they are a great entry point!


![OSWP1](/img/oswp/oswp1.png)
It has been a pleasant and rewarding experience overall. In this blog post I will share with you my Wireless Hacking journey as well as some tips and tricks to learn what you need to pass this certification.


## The PEN-210 Experience

>PEN-210 (Wireless Attacks) introduces the foundations of wireless network security, exploring common vulnerabilities and exploitation techniques. The course prepares learners in skills related to different types and architectures of Wi-Fi networks, wireless reconnaissance, and exploiting vulnerabilities in WPS.

After doing OSCP I have developed a great methodology to learn anything, hacking or non-hacking related, based on note-taking with Obsidian. Having a good and reliable methodology is the most important step in my opinion, so keep that in mind from the first minute that you start the certification. I might write a post about my methodology some day... 

Take good notes and make cheat sheets that allow you to go faster and waste as least time as possible. Also, learn various methods to perform the same attack, as you could get different results with different tools.

- - -
## Exam Structure and Preparation

While I am not allowed to deeply discuss what you are going to find in the exam, I can confirm that the course has everything you need to know to pass it. BUT, after finishing the content I needed more. That's when I discovered WiFiChallenge Labs. Big shoutout to [r4ulcl](https://github.com/r4ulcl) for creating this magnificent resource.

Here is the link of [WiFiChallenge Lab](https://lab.wifichallenge.com/) if you want to take a look.


![OSWP2](/img/oswp/oswp2.png)


Practicing for OSWP is a bit tedious, as you need a WiFi antenna that supports monitor mode and an Access Point that is capable of set the multiple exam environments that you are required to exploit. Here is where the WifiChallenge Lab comes in handy, as it let's you test everything on a Virtual Machine without the need of expending extra money.

But still, if you can afford it, I highly recommend to go ahead and set up your own lab environments with real equipement.

For the preparation part, I felt the content provided by OffSec was **a bit too concise**. I felt that only prepares you for the exam, and not the real world. That's why I keep grinding with the WifiChallenge, which provided me with much more knowledge. This is not necessary to pass the exam but, at the end of the day, we are here to learn, not just to pass the exam.

I had this same feeling on the PEN-200 course for OSCP. I prepared the OSCP exam with the content from the CPTS from HackTheBox, which was a bit overkill but it was great knowledge.

So, in my opinion, make all the challenges that you can from WifiChallenge, even though if they are not part of the PEN-210 syllabus. This will grant you a better global vision of wireless network and you will be able to have a better understading, which will come in handy in crucial moments, like troubleshooting.

- - -

## Exam day. How was it?

For the exam you have 4 hours to complete the technical part and 24 hours to hand in a report. It took me about 4 hours to complete everything, including report, with all 3 flags, so they give more that enought time. 

To pass you must obtain the flags from at least two of the three networks. To read a flag you first need the AP password, then connect to the network and `curl` the web server that hosts the flag.

To connect to the environments, you need to SSH into a Kali machine and attack from there. They also give you the right to use RDP/VNC to have GUI, but in my experience it was really slow, so I stuck to console.

The exam was what I expected. It it probably the most straight forward OffSec exam, but don't get too confident and make sure that you have great understanding of the concepts before jumping into the exam. I had some conectivity issues and I had to reset the exam multiple times, but it was not a big deal.

Don't stress too much with the report. As long as you are able to explain the attacks, take screenshots and submit both the passwords of the Access Points and the associated flags, you will pass.

### Important Note

> Automated tools ARE NOT ALLOWED

If you use WiFi-Challenge Labs as your practice environment, make sure that you learn how to do the attacks manually, and do not really only in tools like `eaphammer`, `eapbuster` , `wifite` and so on.

Also, make sure to be confident with both Wireshark and Tshark, as I said earlier, the GUI doesn't work flawlessly. 

## Overall Experience. What is worth it?

Yeah! Definitely! But again, I feel the overall experience was amazing, including of course the WiFiChallenge Labs. The experience of searching information, learning, setting real environments and practice in the virtual ones was pretty cool!

On the other hand, this course if not for people who doesn't want to be courious and invenstigate on their own. If you are expecting to get great knowledge only from the PEN-210, this course is probably not for you. 

I'm pretty sure this applies to most certifications, but I will always recommend to go beyond what is required. That's the best way to learn!

It is important to note that I got the OSWP voucher by getting the LearnOne bundle for OSCP, which gives you access to PEN-103, PEN-200 and PEN-210 (KLCP, OSCP and OSWP, respectively). I would not recommend to buy the course on its own, as WiFi-Challenge also has their own certifications for half the price, and you will use WiFiChallenge to study anyway haha.

So again, big props to [r4ulcl](https://github.com/r4ulcl) for this amazing resource and thank you all for reading.

If you have any questions, reach my on any of my social media like [Linkedin](https://www.linkedin.com/in/marcosgarciaarcos/) or Discord (@s3ntinl).
See you on the next one!
 

