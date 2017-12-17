# awesome-hardware
Im trying to gather hardware that respects your privacy and freedom. Right now my main focus has been guys that till the Intel AMT/IME

## Intel Management Engine
### Terms
Disabled - This is ment to signal that the company wiped the drivers and/or set the disable bit in their firmware builds. At this time this does effectively mean the ME is forever disabled and should not be an issue, but it is rather hard to verify and at any time Intel could decide that this is not acceptible and take this ability away from OEMs. To my understanding the Binary Blobs still exist but are not actually loaded when the processor boots.

Neutralized/Neutered - This is most of the IME is physically wiped. There are still pieces there that are required for the processor to boot but things like the Intel FSP are still there. Intel does not really support this and it takes a lot of work on the OEMs part to present machines like this. Intel wont beable to change things in a way that an OEM would have to reverse this process but they can change it in new processors making deployment cycles of updated hardware longer as the OEM has to start the process all over again to figure out what is needed to make the system work with a Neutralized IME

Removed - This state no one has got to yet. This is all of the AMT/IME stack is gone and never to return. If you had tools to scan the firmware portions of your board and processor you would see that the place where the IME OS resided is blank. Intel does not provide a way at all to do this and it has been the bane for a lot of OpenBIOS projects.

### Disabled

* [System76](https://system76.com) - These guys love linux and put out their own distro. After the rash of security vulns they did a deep dive and discovered that Intel allows OEMs to effectivly neuter and disable the IME, so they did it. This isn't as far as companies like Purism have gone but it is fairly close.
  * http://blog.system76.com/post/168050597573/system76-me-firmware-updates-plan has a lot of the details about what they did to the IME

### Neutralized

#### CoreBoot

* [Purism](https://puri.sm/) - Purism's products were designed from the ground up with privacy and freedom in mind. They have hardware switches to physically turn off the mic, camera, and wifi. You can also order them without wireless, and with a USB stick so you can airgap QUBES os on it. The BIOS has been replaced with CoreBoot and the Intel Management Engine has been neutralized. The processors are still a bit older due to the complexities in neutralizing the IME but they are probably the newest machines you can get where the IME is neutralized.
  * https://puri.sm/learn/intel-me/ purism's info on what they have done to neuter the IME

#### LibreBoot

* [Ministry of Freedom](https://minifree.org) - They refurbish older thinkpads (t400, x200) and replace the BIOS on them with libreboot. These have earned the FSF Respects Your Freedom seal of approval.
* [TechnoEthical](https://tehnoetic.com) - These guys refubish the older thinkpads (t400, t500, x200) and replace the BIOS with libreboot. All of their products also hold the FSF RYF certifcation.
* [Raptor Engineering](https://www.raptorcs.com) - Raptor Engineering is bringing us the worlds first front to back open computer based on the Power9 architecture. They are using libreboot and since the Power9 architecture is totally open there are really no surprise nasties or gotchas here for Raptor to have to work around.
