---
layout: post
---

A few months ago, I decided it was finally time to install a SSD into my computer. My biggest reason for this was to decrease the startup time, as I would be switching on my computer 30 minutes before I started my working day so I could be sure everything was up and running properly.

## Ordering

Finding a good fit for my computer was pretty simple thanks to [User Benchmark](https://www.userbenchmark.com/Software). The site listed various SSD's, but the one I was drawn to was the [Samsung 870 EVO](https://www.samsung.com/semiconductor/minisite/ssd/product/consumer/870evo/). For my purposes, I didn't need a lot of storage space, so 250GB was plenty. The price seemed reasonable too - just £40.00 to improve the boot time, nice!
I needed this to be a 2.5 inch drive too, as my motherboard does not have a m.2 slot.

I would expect most people to head straight to Amazon to order a new PC part, and understandbly so because of the convenience. However, working in the retail industry has made me realise that local businesses need our support - especially in the midst of a pandemic. Unfortunately for me, if local businesses are suffering, then my employer is suffering too which leads back to me. Therefore, I make every effort to avoid ordering from Amazon and prefer to browse [Google Shopping](https://shopping.google.co.uk/) for parts instead.

Naively, I expected the SSD to arrive with mounting screws and a SATA cable for an easy installation. Of course, this wasn't the case. So one call to a family friend and another order for a SATA cable later, I was finally ready to install my new fancy SSD.

## Installation

Am I going to admit to thinking the SSD would slot in to the space where a floppy disk drive would be in a case here? No, I don't think I will.

After some research, I eventually worked out that the SSD would fit into my case, just not where I thought it would go. It also explained the extra screw holes and vents on the side of the computer case! The power cable wasn't quite long enough to have a tidy route from the power supply, so I needed to make another quick order for a SATA power extension cable.

Finally, the SSD was in the case and working.

## Migration? Cloning? I just want to boot from the SSD!

"Samsung SSD's come with easy to use migration software to make the migration process simple!"

That isn't a direct quote but this is the impression I had. However:

* I wanted to keep my old HDD in the computer as it had room to stay and plenty of storage space.
* The old HDD had a larger storage capacity than the SSD.

Unfortunately, trying to figure this out online proved to be difficult, as most people appeared to want to **replace** their old HDD with the SSD.
I tried moving a lot of files onto my other, much larger 4TB HDD to make cloning work. I waited hours upon hours for the clone process to run, but every attempt wouldn't allow me to boot from the SSD!

I now know this is caused by the boot manager settings also being copied across, because of course, the data has been **cloned** completely. The boot manager needed to know which drive it was booting from, but that data didn't exist on the new SSD as far as it knew.
If you really wanted, you could use command prompt commands to access the boot manager and switch around the letters etcetera. Thinking about it though, this doesn't make sense.
The HDD would have been optimised as part of the Windows 10 installation. A SSD would also be optimised as part of a Windows installation, but these two optimisations would not be the same.

After all of this, I am now sat here writing this post on my new Windows 10 installation which boots from the SSD. It took some setup, sure, but the files I need are still on the old HDD which I can access if I need to. I highly recommend a package manager such as Chocolatey for managing your app installs, as this made installing them onto the new drive much easier.

So, to conclude, if you are getting a new SSD and **not** intending it to replace your old HDD, then save yourself time and a headache and just put a new Windows installation on the SSD. If you have one, your Windows licence key should be picked up from the old HDD when installing.

Thanks for reading!