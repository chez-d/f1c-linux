# f1c-linux
This is a little breakout I made for Allwinner's F1C100s/200s a while ago, also known as the "potatoboard" (it's a 533 MHz ARM9 CPU).

This chip is pretty amazing in terms of cost -- for a couple of $$ you can get really impressive performance, at least if you ignore floating point, and up to 64 MB (!!) of DDR as SiP, so no annoying routing to be seen. This board is designed for JLC's low-cost 4 layer boards and you can even get it assembled by them for pretty cheap, go check out the `fab/` folder for the gerbers and POS files!

I used LDOs on this design so I don't have to deal with switching regulator headaches... so not so great power usage.

Upload to the SPI NOR with the USB connector and the handy `sunxi-fel` tool, or you could try and hook up a SD/MMC card on the GPIO. It even runs Linux!
