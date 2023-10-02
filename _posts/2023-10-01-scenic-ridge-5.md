---
title: "Scenic Ridge: First Blood - laying track down"
date: 2023-10-01 18:03:00 +0800
categories: [ "Scenic Ridge" ]
tags: [ "Scale,N" ]
---

Today, both the [Atlas Scenic Ridge Track Pack](https://www.trainz.com/products/atlas-2588-n-scale-scenic-ridge-track-pack) and the [Atlas 44589 Union Pacific U25B Locomotive (with DCC)](https://www.trainz.com/products/atlas-44589-n-union-pacific-u25b-ph-2a-locomotive-637-w-dcc-ln-box) arrived, so I needed to get down to business laying track down to see if it worked.  First off, here is the track pack on the layout:

![The Atlas Scenic Ridge Track Pack](/assets/2023/1001/img1.jpg)

And here it is without the box.

![Unboxed track pack](/assets/2023/1001/img2.jpg)

The major concern were the track joiners.  They arrive in strips of four joiners, so you have to cut them up to use them.  I have [a pair of snips](https://www.amazon.com/BOOSDEN-Crafting-Electrical-Precision-Clippers/dp/B0936HH4YG) (a similar style - I have not purchased these - but they are cheap enough for a tool).  So I got to clipping those track joiners apart:

![Tools for clipping track joiners](/assets/2023/1001/img3.jpg)

Another major concern was that none of the track was labelled. Since guessing at the track pieces during construction is a bad idea, I decided to label the box they came in:

![Labeling the box](/assets/2023/1001/img4.jpg)

I started in the center (which was a mistake - think where you want the last join to be and start there), and after a bit, I
 had visible progress!

![The first curve laid down](/assets/2023/1001/img5.jpg)

I stopped at this point.  Why, you ask?  Firstly, I **detest** those track joiners.  They really are the worst thing imaginable.  By the time I had finished the first corner, my thumb was bloody.  That's because you have to push the track joiners onto each rail and your thumb is easily the best tool for the job; or the worst depending on your point of view.  I went and covered the cuts with a band-aid, and continued.  The second problem with the track joiners is that they don't all "work".  Some of them just refused to go onto a rail.  Inspection showed that they had been crushed slightly compared to the ones that did work.  Was that me or shipping? Probably me, but I'm not going to stop complaining about these things.

Maybe that's why a lot of people recommend the Kato track?

![More layout](/assets/2023/1001/img6.jpg)

Another problem with the Atlas track is that the small pieces (the 1 inch and 2 inch straight pieces primarily) don't have fixed tracks.  As you push the track joiner onto them, they have a tendency to move.  Putting the end against the wood so you have something to push against solves that.

My final problem is the siding area. The provided pieces just didn't make any sense.  If you went with the provided plan, you got all the right things happening, but in the wrong place, resulting in the siding area being too close to the main line.  If you adjusted according to what is laid out on the board, you couldn't complete the layout.

![The siding area](/assets/2023/1001/img7.jpg)

I was going to change this area anyhow, so it's not a complete loss.  However, it means I'm not going to be able to call this "done" until some more parts arrive, including more of those annoying track joiners.  I need a right-hand turnout and a few more lengths (probably one pack) of the 5 inch straights to complete the set. In addition, I'll need a few more feeder joiners to wire everything up.  I'm sure this set would work with just one feeder if I was using a standard throttle.  I'm using DCC, so all the tracks need to be powered.

I swapped out a set of joiners on the main track with the feeder joiners that were supplied in the kit.  Then I connected a power plug to the end of those so I could feed power to the line.

Since [I'm using DCC-EX]({% post_url 2023-09-30-dcc-ex %}), I had some connectivity to deal with:

* The micro USB on the Arduino board was connected to my PC.
* The 18V power supply was connected to the Power output on the motor shield.
* The feeder joiners were connected to the main track output on the motor shield.

Once that was done, I went to [EX-WebThrottle](https://dcc-ex.github.io/WebThrottle-EX).  You need a Chrome-based browser for this to work.  I'm using Microsoft Edge (which is Chrome based), but use what you like.

![The EX-WebThrottle site](/assets/2023/1001/screenshot-1.png)

Once done, you can select a serial port (from a list of the serial ports recognized), then click "Connect DCC++ EX". Once connected, you can turn the power from off to on.  This will light up the four LEDs on the motor shield, showing it's ready for action.

Finally, select a locomotive by typing its ID in the box, then pressing the button beside it.  My locomotive has not been configured yet, so it arrived as ID #3.  I'll re-program it as ID #637 (which is its locomotive number) when I get some time.  Once I had done that, I could use the throttle just be moving it up and down (either with the two buttons either side, or just by clicking somewhere on the slider).  I could also go forward and reverse or stop by pressing the buttons to the right of the throttle.

Here is some video of the locomotive making its way around the track!

<video width="640" height="480" preload="auto" controls>
  <source src="{{"/assets/2023/1001/trains.mov" | relative_url }}" type="video/mov"/>
  <source src="{{"/assets/2023/1001/trains.mp4" | relative_url }}" type="video/mp4"/>
  Your browser does not support the video tag.
</video>

If you have followed the instructions for joining the EX-CommandStation to Wi-Fi, you can also use an iOS throttle like [SRCPClient](https://apps.apple.com/us/app/srcpclient/id1495402734) (which is free) or [WiThrottle](https://apps.apple.com/app/id344172578) (which costs $9.99 on the iOS store).  I used SRCPClient and found it easy to start running trains.

Now I've proven out the positioning of the risers relative to the actual track, I can dismantle the track and the top level of risers.  Once I've done that, I'll be laying the lower level of risers down.  But that's next time.
