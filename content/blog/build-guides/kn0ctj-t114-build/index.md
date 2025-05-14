---
date: 2025-03-17
title: Heltec T114 Build
author: Calvin Jutting ([@KN0CTJ](calvin@iowamesh.net))
---

## Heltec T114 for Everyday Carry

When I first got started into Meshtatsic I ended up with a few of the Heltec V3s. They were inexpensive and got me out to Vegas in a hurry. I was always annoyed by the battery life and just seemed so sluggish that I started to stray away from them and started going exclusively RAK wireless for base stations, Solar and carry nodes. I was stocking up on my supply Rak Wireless boards and took at chance on the Heltec T114. I had co-workers that were testing them with success so I thought I’d dip my toes. It was based on an NRF processor so it should at least have a good battery consumption.

So here we are with a base install of Meshtastic:
{{< imgproc "t114-shell.jpg" Resize "300x" >}}

Full transparency, Muzi Works does sell a kit that does the same thing. I had ordered the board before finding the kit or the 3d prints so I opted to just get the battery from them and 3d print the case. They were generous enough to post their STL files on Printables! Hats off to them for that!

[Muzi Works T114 H2T Kit](https://muzi.works/products/h2t-complete-device-heltec-t114-with-gps-running-meshtastic?srsltid=AfmBOopTr1Ul0xTtDU487NkT8qcOsMRJxu4_BYPfuo4JvyaMcmVbc319)

Parts List:

[Heltec T114 (Rockland)](https://store.rokland.com/collections/heltec-products/products/heltec-mesh-node-t114-with-optional-1-14-inch-tft-display)

[Amazon Generic Lora Antenna](https://a.co/d/24lYvXB)

[3d Printed Case](https://www.printables.com/model/982046-h2t-case-for-heltec-t114-with-gps-running-meshtast)

[H2T Battery](https://muzi.works/products/h2t-battery)

I had some of these parts lying around from other builds so feel free to swap out what works for you!

{{< imgproc "t114-parts.jpg" Resize "500x" >}}

The first step was to install the antenna cable and route it through the channel they’d built. Hats off the Muzi Works guys for thinking about that as with other builds has the cable in the open. Once in there, you can screw down the connector to stay.

{{< imgproc "h2t-antenna-route.jpg" Resize "500x" >}}

The second step was to remove the two screws that held the plastic shell and screen in place. The screen will be free to move around so be careful not to rip it off or somehow bend it. While the front of the case is face down, put the buttons in, hook up the antenna to the port on the board and put the two little screws in. This took me a few times because while the screen was loose it didn’t work to cooperate the first time times. Be patient and you’ll get it

{{< imgproc "t114-screws.jpg" Resize "500x" >}}

The next step is to put the battery in the tray. Another feature of the case is a nice way of routing the battery cable so it avoids hitting the antenna and other parts of the board when the case is fully assembled.

{{< imgproc "h2t-battery-route.jpg" Resize "500x" >}}

{{< imgproc "t114-battery-tray.jpg" Resize "500x" >}}

That’s pretty much it. Plug the battery into the battery port (make sure it’s the correct way so you don’t burn out the board) and enjoy. 

{{< imgproc "t114-full-assemble.jpg" Resize "300x" >}}

I have to say I’m impressed with the battery life. I opted to not put in the GPS and use the GPS from my phone when I care enough to do it, but this last just as good as my rak carry (which will be another post soon). It is responsive when you hit the buttons, the screen is easy to read and use and overall a good unit. I’ve not messed with other antenna as of yet, but the Amazon one seems to do the trick. As soon as I get my nanovna I might hook it up and find out how close to 915 it is! 

Thanks for taking the time to read this. I hope it was helpful!
