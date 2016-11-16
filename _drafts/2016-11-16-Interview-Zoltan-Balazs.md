---
layout: post
title: Interview with Zoltán Balázs, security expert
author: mark
author_name: "Mark Felegyhazi"
author_web: "https://hu.linkedin.com/in/felegyhazi"
---

We are more than happy to welcome [Zolt'n Bal'zs](https://jumpespjump.blogspot.hu/), (also [on Twitter](https://twitter.com/zh4ck)) as the next security expert on our blog. Zoli has long track records in bypassing security defense products. He regularly give talks on security conferences such as [DEFCON](https://www.youtube.com/watch?v=ssE_mwSEH9U), [Botconf](https://www.botconf.eu/2015/sandbox-detection-for-the-masses-leak-abuse-test/) or [Hacktivity](https://hacktivity.com/en/hacktivity-2016/presentations/the-real-risks-of-the-iot-security-nightmare-hacking-ip-cameras-through-the-cloud/). He is now working as the CTO for a company creating such bypasses.


Here is his story.
<!--excerpt-->

----


<span class="post question">Mark Felegyhazi: OK, so thanks Zoli for joining us. Why did you start IT security and how did you end up in this very exciting, but very difficult profession? Can you tell us a little bit more about yourself and why did you choose IT security?</span>

<span class="post answer">Zoltán Balázs: </span> I think there were multiple important milestones in how I really started IT security. The first one was when I found the Dodge Viper hacker club which was a very old Hungarian website. They collected all of the tools and know-how for script-kiddies. I really enjoyed that. The next important milestone was the Infosec faculty at the [Budapest University of Technology and Economics](https://www.bme.hu) where I really started to invest my time in IT security. The next milestone was my thesis with Sándor Gajdos. It was about database security. It really helped me to deep dive into one special area in IT security. The next important milestone was when I started to try challenge sites like [WeChall](https://www.wechall.net/). So I was able to practice my skills on different areas in IT security like cryptography or ethical hacking. Last, but not least, what was really motivating to me in the past is when I met the Hungarian ITsec community in 2009.

<span class="post question">MF: Can you tell us a little bit more about this Dodge Viper hacker club? Why was it interesting and how did you discovered it?  Was it an igniting moment when getting from nothing into IT security suddenly?</span>

<span class="post answer">ZB: </span> I think the first time I heard of all these was on IRC. It was just really fascinating for me to see that is really a new world which opened my eyes that there are always constraints what you can do, but if you are creative enough and you have the skills, there is always a way to circumvent these constraints. 

<span class="post question">MF: That's very nice. Would you recommend to newcomers to discover something that they think is solid and then try to circumvent it?</span>

<span class="post answer">ZB: </span> Oh yes. Actually, I think this kind of thinking what really helps to develop the skills.

<span class="post question">MF: So you mentioned that database security for your thesis. Was it your favorite topic at that time? How did it evolve over time, so what is your favorite topic now in IT security?</span>

<span class="post answer">ZB: </span> Well then that was the only field so it was my favorite, but I think nowadays I don't have any single topic which is my favorite. I always enjoyed reading of all malware analysis, antiforensics, opsec and these kind of things but I'm basically interested in everything in IT security which is not about policies and certifications and these kind of things, but otherwise I am always interested. And... Why do I love IT security? I think every day there is something new, something interesting and I really love the cat and mouse game in this whole infosec area. 


<span class="post question">MF: So you said, you don't have a specific topic in mind but you mentioned a lot of hacking and ethical hyping and pentesting thing. So what do you think of ethical hacking as such because there's a lot of controversy about about these questions whether you know it's a weapon. It can be used for good or bad. What do you think about this double edged sword. </span>


<span class="post answer">ZB: </span> I think it was more controversial in the past and my opinion is that for example joining the army is more controversy than being ethical hacker. I think nowadays people understand that in order to fight the bad guys you need skilled good guys. So there is no question about that. 

<span class="post question">MF: So what would you suggest to the newcomers and young people have to stay ethical in this world? So how to pick up the mindset of staying on the good side and not on the dark side?</span>

<span class="post answer">ZB: </span> I think it mostly has to do with how you have been raised as a child and follow the ethics you learned. Sometimes you can see in the news that some black hat hacker after doing some illegal activity became part of a team of a huge company or something. These are mostly fairy tales I think. And it is a lot easier in the long run to just stay ethical and build up your career on the ethical path.

<span class="post question">MF:  So do you think that the team actually makes a big difference if you find yourself in a good team for fighting for a good purpose that this can actually determine your attitude as well towards the system. </span>

<span class="post answer">ZB: </span> Yes, I totally agree. 

<span class="post question">MF: That's awesome. So getting from ethical hacking to your current activies. So as far as I know these days you are bypassing security products. Can you tell a bit more about this and what is the different from the whole generic traditional hacking world and why do you think that this particular subject is really interesting and why do you do it for a living right now? </span>

<span class="post answer">ZB: </span> I think in general bypassing defensive products not just AV is very similar to traditional ethical hacking and sometimes it can be even part of general ethical hacking project. But, let me tell you an interesting and very recent story about bypassing these products. Before the last ethical hacking conference here in Hungary, Buherátor started an ad-hoc hacker challenge on Facebook. The challenges was about to generate a meterpreter-style malware which downloads and executes another exe file downloaded from the internet and executes it locally. The task was that it shouldn't be detected by any of the engines on VirusTotal. First it took me about four hours to figure out what the task is here because it was very cryptic and you didn't know what to do, but after I found it these, actually, it took me like four hours to create such malware which bypassed all the engines on VirusTotal. Although there is a small cheating here because on VirusTotal only a subset of the AV defenses are running. I think it still proves that automated defenses are never enough for new threats.  

<span class="post question">MF: I see. So you say that the skillset is very similar to traditional pentesting. There is not much special you have to learn for this particular product testing and product bypassing.</span>

<span class="post answer">ZB: </span> Yes. 

<span class="post question">MF: Do you also give suggestions on how to improve the products after the testing. </span>

<span class="post answer">ZB: </span> Yes, you know in our company one of our key strategy or message is that don't just break things but we help to fix it. 

<span class="post question">MF: That's very important. We believe also in positive attitude and positive security. And you got very successful with this. As far as I know you got a DEFCON talk on bypassing firewalls and defensive products. How did you get to DEFCON? Could you tell us more about this very nice achievement?</span>

<span class="post answer">ZB: </span> I believe that the reason that I was the first Hungarian speaker at DEFCON, is not because of the sophistication of my topic, but rather of my faith that I can do this. I can tell you at least 10 Hungarian speaker presentations from the past five years which are good enough for DEFCON, but I guess people never tried to send their presentation to DEFCON, because they never thought that they are good enough. I think it's sometimes a problem here in Hungary that people don't believe in their capabilites. 
My message to all the current and want-to-be speakers is that being rejected from a conference is still better than not submitting your talk to the conference. I get rejected a lot of times, but still in a few cases when my talk was accepted totally worth. 

<span class="post question">MF: So the reaction of DEFCON was positive. Did people like your talk?</span>

<span class="post answer">ZB: </span> Yes. Actually I have seen tweets from people I respect. For example, Dan Kaminsiky or @thegrugq, who enjoyed my talk. I was really proud about this. And I have to say that DEFCON is the second best conference I have attended so far right after Hacktivity. But I might be subjective on this part. 

<span class="post question">MF: All right here is the Hungarian bias. :)</span>

<span class="post answer">ZB: </span> Several things in the U.S. are huge. And DEFCON is also huge, but in a new and really exciting way. For me the experience of being at DEFCON was like being in candyland for a child. 

<span class="post question">MF: That's very nice. Let's let's talk about issues in the world. What do you think about security? Where does security is heading right now in the world?  What are the most important issues? I know what you do right now but if you could give us a generic perspective. What do you think are the things we have to solve as security professionals? </span>

<span class="post answer">ZB: </span> First of all, the biggest issue know is to convince management to invest in security. Nowadays, however, at least ransomware is trying to convince people. Actually this is the very first threat which really helps people to understand that IT security is important. The second biggest issue is education, because education can keep up the pace with the number of people needed in this field. 

<span class="post question">MF: You also mean education of new people or the education of existing people like software developers, system administrators, or IT people in general who maybe are lacking the skills needed for today's world security related skills?</span>

<span class="post answer">ZB: </span> I think it's both, because there is a lack of good people and there is also lack of talented people in IT itself, but in IT security the issue is even worse. If we get people from general IT, we don't solve the problem on a global level. 

<span class="post question">MF: So even if we increase the number of people ten times in IT, you will have enough programmers, but it won't solve the problem of IT security, because you have to train thos people to secure development or secure system building in mind, which is very often not done  in school and trainings. </span>

<span class="post answer">ZB: </span> Yes.

<span class="post question">MF: Yeah this is a big big problem actually pointed out by many CEOs including the CEO of Symantec who considers this is the most pressing issue. </span>

<span class="post answer">ZB: </span> But also another issue is that good guys from high school if you don't get good guys from high school the university cannot build upon that. 

<span class="post question">MF: That's true. So do you think that building up an IT curriculum from the very being, maybe even from primary school would be very important to teach people that this is a new world? It's all intertwined with software. They have to use software, or even write software later on. And if you don't teach them from the very beginning then this digital world is going to be a surprise for them and we need more people with digital skills and not just Facebook.</span>

<span class="post answer">ZB: </span> Yes, I totally agree, because nowadays almost every child is playing with computers. 

<span class="post question">MF: Fantastic. So coming back to you. Tell me why did you selected to work for a small company. Partially, your own company, because you are having a key role as a CTO there. Why not working for a big corporation in a pentesting job in pentesting very big systems and exciting systems. Why your own path, your own way?</span>

<span class="post answer">ZB: </span> I started my career at a financial institution with the biggest internal network in the world and while I started changing jobs I started to work for smaller and smaller teams and companies. I think big corporations are good to see how things should be done or sometimes how things should not be done. But if you're working for a small company, you can basically build something new and big corporations are not the good way if you want to create something big or something what is really yours

<span class="post question">MF: It is because they have too many rules, they're not flexible or they're just simply not fast enough to do these new things?</span>

<span class="post answer">ZB: </span> All of these.

<span class="post question">MF: Okay. So if a kid woke you up and asked for your advice about learning security what would be your point? One sentence response to that. </span>

<span class="post answer">ZB: </span> Never stop being curious about how things work and don't be afraid to try and fail before succeeding because those who never fail never succeed. 

<span class="post question">MF: Yeah, any kind of pragmatic suggestions, because I think motivation is the most important. But let's say I'm a kid out of high school and I'm interested in programming and everything. So where do I start? Let's give him the first step. I would highly recommend these challenge sites because you can find the first </span>

<span class="post answer">ZB: </span> I would highly recommend these challenge sites, because you can find a topic which really gets your attention. The more skills you acquire through these challenges, which might be addictive sometimes, the better you can become in every field. 

<span class="post question">MF: All right. that's fantastic. And finally once you got into IT security you use a lot of tools and lot of skills. Can you tell us your favorite tools which is particularly interesting here for us in avatao because this is what we are interested in also. </span>

<span class="post answer">ZB: </span> I think I use more tools than the average IT security guy, but still my favorite is python and powershell. 

<span class="post question">MF: Awesome. </span>

<span class="post answer">ZB: </span> It is not a tool, I know, but ...

<span class="post question">MF: Perfect. Thank you very much. 

