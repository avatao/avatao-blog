---
layout: post
title: Interview with Mateusz "j00ru" Jurczyk, security expert
author: gabor
author_name: "Gabor Pek"
author_web: "http://www.crysys.hu/~pek/"
---

We are more than happy to welcome [Charlie Miller](http://j00ru.vexillium.org/), (also [on Twitter](https://twitter.com/0xcharlie)) as the third security expert on our blog. When talking about low-level Windows kernel security, we are unable to avoid his name. He won the [Pwnie Award 3 times and was nominated 6 times](http://pwnies.com/) in various categories. He is one of the key members of the Dragon Sector CTF team which became the best team in the world in 2014 on [CTF time](https://ctftime.org/team/3329).


Here is his story.
<!--excerpt-->

----

<span class="post question">Gabor Pek (avatao): You have a Ph.D. in Mathematics and you are now one of the best known security researchers in the world. Why did you change your field of interest and why IT security?</span>

<span class="post answer">Charlie Miller: </span>I received my PhD in Math but from there if I wanted to stay in math, I had to continue doing research in the field I had written my phd in.  I didn’t want to continue that research.  In academia, at least for a long time, you can’t easily switch research topics.  Besides academia, there aren’t many jobs out there for a phd mathematician, so I ended up going to work for the NSA which was hiring cryptographers.

<span class="post question">GP: How did you start learning IT security? Where did you get help from at the beginning when you got stuck in a problem?</span>

<span class="post answer">CM:</span> Even though I was hired to be a mathematician at the NSA, they had a variety of training programs.  I started training in computer security and working jobs there that emphasized this skill.  I basically learned on the job, which is a great way to do it if you can.

<span class="post question">GP: You won the Pwn2Own contest at CanSecWest 4 times and were nominated for the Pwnie Award 3 times. These are huge results. What is your
approach to control a previously unknown software?
</span>

<span class="post answer">CM:</span>The most important part is deciding what to do.  Whether that means picking the piece of software (say Safari) or which part of that software to attack (say a particular part of the Javascript engine), focusing on the right parts helps you become efficient at finding vulnerabilities. 

<span class="post question">GP: Most of the products today fail to meet the security best practices to keep up with the business demands. How do you think this controversy could be solved?
</span>

<span class="post answer">CM:</span> I don’t think there is an easy solution.  Companies want to sell products and be first to market.  Security is expensive and, for the most part, invisible to the consumer.  This makes it hard for companies to justify large expenditures in security.

<span class="post question">GP: You are also well-known for your research in car security. What do you think the most pressing issues are in car security today? How do you
envision car security in a few years from now?
</span>

<span class="post answer">CM:</span> There are a few issues that make car security different from most computer security.  For one, the effects of issues are much more critical.  However, the biggest issue is that cars take years to go from design to production.  That means any security lessons we learn now won’t be present in cars for 4-5 years.  This is one of the reasons why it is important to start working on car security now, before we have real world issues, because otherwise it will be too late.

<span class="post question">GP: What do you think are the most pressing issues in OS security today? How do you envision OS security in a few years from now?</span>

<span class="post answer">MJ:</span> I think the one most pressing issue in OS security today are the various legacy design decisions and specific areas of code, which even though were introduced 20-30 years ago, are still running behind the fancy UI's and defining the security posture of modern systems. It is obvious that coding practices and the overall approach to security was completely different several decades ago, but with so many layers of new code and design built around the old ones throughout the years, it has now become very difficult to fix them. This is especially true since operating systems are widely expected to maintain backward compatibility, which often stands in the way of improving security.
<br>
On the other hand, it is impressive to see all major vendors put a heavy emphasis on OS security in the recent years. Since Windows is my area of expertise, I will use it as an example: the system not only has all externally reported bugs fixed, but with each new iteration, a tremendous amount of general improvements are added, mitigating entire families of bugs. For instance, Control Flow Guard makes it considerably more difficult to exploit use-after-free vulnerabilities, moving the font renderer to a sandboxed user-mode process reduces the impact of any font exploits and makes them much less attractive, blocking access to win32k.sys system calls for specific processes eliminates a whole giant attack surface and so forth.
<br>
Seeing how challenging it already is to fully compromise a system with just memory corruption bugs, I think we might see a visible shift towards logic bugs in the upcoming years.

<span class="post question">GP: What do you recommend how the next generation should start learning IT security?</span>

<span class="post answer">MJ:</span> Finding or starting a CTF team and participating in competitions is definitely a good way to kick off, as you can usually find a very diverse set of tasks at all levels of difficulty. In addition to mastering strictly practical skills, I would also recommend reading as many technical security books, articles, blog posts, conference slides and whitepapers as possible. They provide a very good insight into the current state of the art, are immensely inspiring and help getting into the specific hacking mindset.
<br>
On a related note, both [Parisa Tabriz](https://medium.freecodecamp.com/so-you-want-to-work-in-security-bc6c10157d23#.j1pnq71qf) (that we [blogged about earlier](https://blog.avatao.com/Your-first-avatao-Tuesday/)) and [lcamtuf](https://lcamtuf.blogspot.com/2016/08/so-you-want-to-work-in-security-but-are.html) have recently published their thoughts on the subject, and I fully agree with both write-ups.

<span class="post question">GP: And finally. What are your favorite tools?</span>

<span class="post answer">MJ:</span> For any kind of reverse engineering and debugging, I love the all-time classics: [IDA Pro](https://www.hex-rays.com/products/ida/) with Hex-Rays decompilers, [WinDbg](https://msdn.microsoft.com/en-us/library/windows/hardware/ff551063(v=vs.85).aspx) and [gdb](https://www.gnu.org/software/gdb/) with enhancement plugins such as [peda](https://github.com/longld/peda) or [pwndbg](https://github.com/pwndbg/pwndbg). I am also a huge fan of [AddressSanitizer](https://github.com/google/sanitizers/wiki/AddressSanitizer) (and other sanitizers from the family: [MSan](https://github.com/google/sanitizers/wiki/MemorySanitizer), [TSan](https://github.com/google/sanitizers/wiki/ThreadSanitizerCppManual) etc.), as it makes bug discovery, crash deduplication and root cause analysis so much easier for open-source software. Finally, I really enjoy using the [Bochs x86 emulator](http://bochs.sourceforge.net/) where I can, thanks to its very convenient instrumentation API, compatibility with latest CPU features and ability to instrument entire operating systems.

----

Follow j00ru's footsteps into reverse engineering and try yourself at these avatao challenges: [R3v3rs3 2](https://platform.avatao.com/paths/2bf3c9cb-f759-4915-9a2f-f30164c45fce/challenges/d80d53ed-597a-4b7e-9897-b85784489029), [R3v3rs3 4](https://platform.avatao.com/paths/2bf3c9cb-f759-4915-9a2f-f30164c45fce/challenges/b82ef4d6-35e8-4330-9155-9eedd332833d).