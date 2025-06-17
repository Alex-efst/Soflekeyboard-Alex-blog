# Soflekeyboard-Alex-blog
This a blog style documentation of how I built my first split keyboard Sofle v1.

# Introduction & Motivation
I decided I'll document my attempt at building a Sofle v1 because I found very few people document their progress in details, which lead me to have very little reference to comapre to and guide myself through on how to build this. To be fair, there's a guide [you should definitely read](https://josefadamcik.github.io/SofleKeyboard/build_guide.html) but I found it lacking for somebody who has 0 prior knowledge on building electronics and it won't show hurdles you might face.
This my first PCB soldering and my first attempt at working with soldering iron was trying to fix my audio cable for my speakers.

# Preparation 

For somebody who's in EU, I found it difficult to find something within a reassonable price to buy a kit from. I could have bought every individual part separately but I found that the shipping cost from different vendors varied quite a lot. In the end, I bought it from [Beekeeb](https://shop.beekeeb.com/) where I heard there was at least some support too in case things got rough (which I ended up using).

My guiding material was the guide mentioned before but [Hexxor](https://www.youtube.com/@Hexxor) on youtube made a [playlist of livestreams](https://www.youtube.com/playlist?list=PLb7Sm5pkDMmUcZOBVjPqtzNx2sZXQhnyk) of how they built a keyboard from start to finish, which I highly recommend you follow as I'll be mainly doing the same here.

## Set up
![IMG_20250427_143044](https://github.com/user-attachments/assets/0931a2d2-07fa-4e20-ad1b-76c00813c15d)
* I fail to recall what soldering iron I'm using but it was 20€ ish kit which you see bundled everywhere.
* My phone for extra light (Flashlight mode)
* A cut up sponge for dishes & extra soldering tin (1m thick, I would advise for smaller for finner control)
* A case fan (F12 PWM Artic) cut up to a USB cable to power up (Don't expect much suction, it's just enough to put the tip in front to suck up the fumes)
  * If u wanna do the same, the wiring should be the same for most case fans, I did have some trial and error to get it right.
    
    https://support.arctic.de/en/f12-pwm-pst
    ![Pc fan](https://github.com/user-attachments/assets/453be5f0-43e6-4987-a9c5-448e24250ada)

Later on I got an small upgrade
* Soldering stance with helping hands, magnifying glass and a soldering iron stand (Goobay 51226). I ended up not using it but it was more stable for resting my soldering iron, it does lean a bit forward so for those with a keen eye, I did get a backup and strap it on the stand to use as a counterweight.
* A multimeter (UT131B) which I highly recommend as you will need to do testing.
* Solder wick braid, which I did use with some flux from the kit
![IMG_20250617_140953](https://github.com/user-attachments/assets/bafbfd5d-ab96-4960-8380-29f88d63b3af)

# Building
I'm gonna use a very common quote and one mentioned on the guide.
> _**Think twice, solder once**. Desoldering is frustrating and it’s easy to mess up things._

I honestly couldn't agree more, which is why I ended up having to watch the playlist for the part I'm working on, then have it on my phone to reference while soldering and plan my steps in details to how I'm gonna solder.
Other then that, I wanted to make this keyboard for the shake of learning so I did plan that I'll make mistakes (and I did) and I did it on my own pace to be sure to that I'll have fun.

## Diodes
It's fairly easy to understand, take arrow from PCB and match it with the diodes. I did struggle to understand what they do and if the diodes I had were looking in the right direction but after checking livestream and some reference images, it felt like I was paranoid over nothing. 
As Hexxor mentions (livestream), a good technique of soldering parts is:
* Have one side with a little bit of solder on the pcb
* Put the part on top and heat up the tin on the pcb for it glue on.
* Solder the other side with generous amount of tin to work as a physical support (I personally ended up doing both sides due to my inexperience and fear of having to troubleshoot later)

### Testing
Here's where I needed a multimetter, it's roughly 0.56V.
Initial, I couldn't get the multimetter to work for diode testing, I found out that you need to press a yellow button to alternate between modes (not mentioned in manual :<).
Other common problem I had was that I put too much tin on the connections, so i ended up having to re-do them by marking them with tape ![IMG_20250616_203659](https://github.com/user-attachments/assets/4dc12f5d-e91d-4459-b070-7e79c2e5cf8d). 
I even found 2 diodes that I placed with the wrong polarity.

## Sockets for switches
You place them like this on the backside (same side as diodes) ![IMG_20250617_145052](https://github.com/user-attachments/assets/982a3324-0299-47dd-af40-ce67e678f3a5)
Using the same technique as I did before (somewhat forgot and ended up remembering it again), it's somewhat more difficult as you're obstructed by the socket but with more generous amount of tin it's easier to glue on the pcb.
Results were this, with me forgeting one thump socket Q_Q.
![IMG_20250617_181903](https://github.com/user-attachments/assets/d2d082b4-67a9-4b3a-af9c-303ca0971dd1)
