## Purpose of Document
This is the transcript of a Slack conversation on September 2nd, 2017 with Gabriel Luong (@gl), a Mozillian who has helped UCOSP students get started on Mozilla.
```
10:48 AM
ellis: @gl I'm just checking in. Might you have some direction as to the environment that we should be investigating? For instance, do we need to build Mozilla from the ground up?
gl: @ellis let me send you some stuff
ellis: !gl, wonderful! I'm prepping for class next week and have Michael who will help other students get started.
gl: @ellis I am gonna start a google doc and share it with you and take content from my previous UCOSP session
ellis: Wonderful!!!
@ellis https://docs.google.com/document/d/1XCyK8CVVgnwqLrKCYYa2JWlc1Lk31Sz_V6fnyLybi-M/edit?usp=sharing
it's gonna be a WIP
there's multiple steps in getting setup
including the development environment
ellis: Right, I expected multiple steps.
gl: the bullet points are usually things that i would demo to people
i will need to double back
and expand on them
later
ellis: @gl Sure, that's fine.
@gl Do we need to build from the ground up from m-c?
gl: @ellis not necessarily, you will have to clone m-c, but there is artifact builds that would really save you time
ellis: @gl  Thank you!!
@gl Yura suggested that improving screen reader keyboard navigation and semantics in DevTools would be a good area.
gl: @ellis I would have typically prefer to have gone through the steps of our development environment setup in http://docs.firefox-dev.tools/getting-started/build.html#using-git
@ellis but i feel like i might be rushing a bit
Ellis: @gl Got it.
@gl To clarify, Michael is a student helper and he is walking through the steps.
@gl  So I have some help and someone to try things before the class.
@gl Michael has cloned from m-c following the instructions for windows using visualstudio, etc.
gl: @ellis I am curious which development setup guide Michael is following and have they been successful?
ellis: @gl he has been working from: https://developer.mozilla.org/en-US/docs/Mozilla/Developer_guide/Build_Instructions/Windows_Prerequisites
@gl And currently he is getting an error about not having a C compiler. I think this is a path issue as he has one installed via Visual Studio.
gl: @pbro ^ do you have any guides for installing on Windows
pbro: @gl other than what is on MDN, no. When I installed on Windows, I followed the official "building Firefox" page I believe: https://developer.mozilla.org/en-US/docs/Mozilla/Developer_guide/Build_Instructions/Simple_Firefox_build
which has links to specific Windows stuff
gl: @ellis I believe http://docs.firefox-dev.tools/getting-started/build.html#using-git should work for linux and mac, but definitely not for Windows
ellis: @gl Ah, thanks.
@gl Any idea if that build has anything that prohibits it being used in a VM?
gl: @ellis in my google doc, I have basically 2 build paths that I did with my student. The first way was to just do a regular build that includes compiling the platform C++.
ellis: @gl Ah, this is all really helpful!
gl: @ellis but typically for developing for devtools, you don't need to do compile the platform C++.
ellis: @gl  Got it.
gl: @ellis but when i was instructing my students, i wanted to show them all the workflows should they want to contribute to platform C++ one day
@ellis the easy workflow with using git is to do https://github.com/glandium/git-cinnabar/wiki/Mozilla:-A-git-workflow-for-Gecko-development
GitHub
glandium/git-cinnabar
git-cinnabar - git remote helper to interact with mercurial repositories
@ellis This should be equivalent to the script you see in http://docs.firefox-dev.tools/getting-started/build.html#using-git
but I haven't dogfooded it myself
ellis: @gl And I'm assuming that we could contribute any changes that we find that we need, back to documentation?
gl: yes for sure
ellis: :slightly_smiling_face:
gl: i am sorry there is just a lot of docs everywhere
one method doesn't necessarily work with windows as well
so, it's complicated
ellis: @gl Yup, your input in finding our way has been very helpful.
gl: @ellis the most definitive guide most engineers use in mozilla is https://github.com/glandium/git-cinnabar/wiki/Mozilla:-A-git-workflow-for-Gecko-development (Works for Mac/Linux)
but this guide itself won't set you up to do artifact builds or mozreview
ellis: @gl thanks!
gl:  @ellis so, my general recommendation for now is to get ./mach build and ./mach run to work
ellis: @gl  @mhawes is the student working on the installation.
@gl great!
gl: @ellis @mhawes once you get ./mach bootstrap, ./mach build and then ./mach run to work
and you see firefox running
you can add on mozreview and artifact build
ellis: @gl and then nirvana happens!
gl:  this both requires editing some configuration
this is the guide to add artifact build https://developer.mozilla.org/en-US/docs/Mozilla/Developer_guide/Build_Instructions/Artifact_builds
during ./mach bootstrap you can specify to go straight into working with artifact builds
which is also what i would recommend
instead of doing what we call a full build
which would compile the c++
ellis: @gl Got it.
gl:  but to do artifact builds, you have to use git cinnarbar
which is a git-wrapper over hg
@ellis @mhawes i would recommend sticking to Slack for communication and Git for everything else
ellis: @gl great, very helpful.
```
