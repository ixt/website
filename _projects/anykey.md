---
layout: post
permalink: /anykey/
title: Press Any Key To Continue
date: 2015/04/30
colour: green
type: installation
---

PRESS ANY KEY TO CONTINUE is an installation commenting on the oversimplification of interfaces and the blind acceptance by the user of these interfaces. The piece comprises of a CRT monitor, webcam, printer and a single key keyboard.

---

## Documentation

---

I wanted to create a single button computer that requires interaction to work, that had random fuctions, patterns and sounds orginally.

-- Composite and Drawing 01

I mocked up these rough images to show  roughly what I wanted the first sight to be. A big smily inviting computer with a single button that just invites you to press it.

-- 2 Face Screenshots

I created a few different faces first trying to replicare the same sort of feeling as the apple mac face but couldnt quite get it right at this stage.
I knew after a while of theorising and playing round with the different visuals that I wanted to use OpenCv to detect that people were sitting there so I began playing with counting faces and having visuals react to if a face was there or not.

-- Drawing 02

I drew the above test face to help out when I needed multiple faces on camera at once (due to my unfortunate position of being awake at 4am coding and only having a single face myself).

-- Test Screenshot

I started working on various individual parts of the overall piece.
I ordered a selection of Cherry MX Switches to choose the best suited feeling and sound for the single key and looked into OSU keyboards (OSU being a rhythm game) which have 2 keys, most were made DIY with either a Teensy or a Trinket, I ordered a Trinket and found the Adafruit Trinket Keyboard Sketch, Modified it to my needs and then when the switches got here, soldered up the most appropriate (I tested: red, black, blue, green, brown, clear) which turned out to be a clicky tactlie green switch.
I also ordered a custom printed keycap with Any Key wrote onto it but these detracted from the piece so I didnt use them in the final use of it.

-- Key making process

Above are images from cutting out the hole in the base and testing a switch fitting in (shown mx clear)
Below are the final product with trinket soldered and installed (along with mini to micro usb right angle adapter)

-- Key making process cont.

I kept an eye out for CRT monitors as it was pretty crucial to the aesthetic I wanted to make, eventually I got one and cleaned it up.
I had some sound clips and a wordlist to match them already recorded/wrote from a previous project and on a hackday I assembled a simple poetry generator ( https://www.hackerleague.org/hackathons/hacksmiths-mini-hack/hacks/poetry-test-slash ), on this hack day I also got processing to send a command via a bash script to Lynx, the text based browser, to send back and read a webpage in plain text this was used to be visualised on screen.
The printer was reletively straightforward, after learning about CUPS existance and how to send prints via the console (with the previous experience with the bash scripts) I was able to get the files printing pretty easily via the lp command. This could have been made automated to select a printer but I didnt think it was nessecary for the lifetime of the piece.
Setting up a function so that after a certain time the button would also save a picture from the webcam when pressed allowed the piece to take on a more sinister tone and allows me to look back on the reactions of the users from the position of the piece some of the pictures from the opening night are shown below.
Although the printer & opencv ran well on my macbook, an early plan was to use a raspberry pi 2 to run the piece on, as the program wasnt too heavy and should technically support linux. I did get the sketch to run in its most basic forms, producing some sound and some visuals, OpenCV didnt work correctly and the Printer I was going to use did not have ARM drivers so this was pretty much impossible. I spent a while trying to get the printer to work as I saw this as being more important than the Open CV aspect. When things started to look grim and I couldnt understand how postscript drivers work I gave up on the Pi2 and refocused on improving the experience under MacOSX.
Next I deveoped a filter that move the pixels of the entire sketch to a colour listed in my 18 colour colour pallete (CGA + 2 Oranges). This gave the piece more of a retro look and broke more of the nice looking visuals into weird visuals that didnt quite look fantastic but suited the theme pretty well.

-- Screen shot blurry

After a while the face being displayed on screen often would interfere with the sketch visually either by actually mixing in effect (above) or by just not working well aesthetically. Removing the face, although it had been in from the start, was a tough decision and did take back some of the charm but I believe it was the right decision not to personify the piece but to make it almost like a mirror with no personality of its own just a reflection of the user.

-- Youtube link / embed

---

-- Photos from exhibition

As seen above the piece once insitu did attract and get people to interact with it.

-- View from user

View from user (above). View from piece (below)

-- View from piece

What I found particuarly interesting was that once people started to realise that if you spent long enough with the piece you got a print of a photo of yourself they would stay interacting or come back with friends to take a group photo. One group in particular coloured in their prints and cut out some too collaging (unfortunately the photo below is the best shot I have of it)

-- More Views from piece

All images I took on site with glass and the images the piece took from that night and the next day can be downloaded here < Link to zip of all images collected