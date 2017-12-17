# awesome-hardware

## Intel Management Engine Disabled
* [System76](https://system76.com) - These guys love linux and put out their own distro. After the rash of security vulns they did a deep dive and discovered that Intel allows OEMs to effectivly neuter and disable the IME, so they did it. This isn't as far as companies like Purism have gone but it is fairly close.
  * http://blog.system76.com/post/168050597573/system76-me-firmware-updates-plan has a lot of the details about what they did to the IME

## Open BIOS/EFI

### CoreBoot

* [Purism](https://puri.sm/) - Purism's products were designed from the ground up with privacy and freedom in mind. They have hardware switches to physically turn off the mic, camera, and wifi. You can also order them without wireless, and with a USB stick so you can airgap QUBES os on it. The BIOS has been replaced with CoreBoot and the Intel Management Engine has been neutralized. The processors are still a bit older due to the complexities in neutralizing the IME but they are probably the newest machines you can get where the IME is neutralized.
  * https://puri.sm/learn/intel-me/ purism's info on what they have done to neuter the IME
* Most ARM devices - It is worth noting most ARMv7 and newer devices either directly use coreboot or use an offshoot of coreboot that is still open. Depending on how open and free you want your hardware ARM without trused/secure boot is generally a safe bet. Also at the same time if you are really concerned about Open Hardware keep away from anything with a Broadcom or Samsung chipset for the most part their specsheets are very much closed and require an NDA to see.

### LibreBoot

* [Ministry of Freedom](https://minifree.org) - They refurbish older thinkpads (t400, x200) and replace the BIOS on them with libreboot. These have earned the FSF Respects Your Freedom seal of approval.
* [TechnoEthical](https://tehnoetic.com) - These guys refubish the older thinkpads (t400, t500, x200) and replace the BIOS with libreboot. All of their products also hold the FSF RYF certifcation.
* [Raptor Engineering](https://www.raptorcs.com) - Raptor Engineering is bringing us the worlds first front to back open computer based on the Power9 architecture. They are using libreboot and since the Power9 architecture is totally open there are really no surprise nasties or gotchas here for Raptor to have to work around.
