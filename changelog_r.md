## Build Information
```
Kernel: DragonHeart Kernel
Type: Bleeding Edge
Device: OnePlus 7/T/P
Compiler: Eva GCC 12.2.1
Branch: staging
Build Number: r16b6
```
## Changelog
**-r16b6**

* Grab all recent FOD improvements from John.
* Update in-kernel LZ4 to v1.9.4
* Fix crashdumps for ESOC devices permanently.
* Increase rating of teo governor to 50.
* Save power when connecting to an USB.
* Disable QCOM download mode.

**-r16b5**

* Reset hard to r16
* Grab relevant improvements.
* Grab PD / Passthrough fixes.
* Grab FOD improvements from John.
* Grab SSR fixes from John.
* Nuke techpack/data to fix wlan perf.
* Fix BSOD.
* Nuke MGLRU.
* Nuke slmk tunables.

**-r16b4**

* Grab a MGLRU fix.
* CFQ tweaks.
* Misc TCP tweaks.
* Reverts done to fix DSOD completely (considering it seems to be a SCSI issue).
* Enable GC for wakelocks.
* Drop SLMK min reclaim.

**-r16b3-hotfix**

* Fix offline charging.

**-r16b3**

* Roll back to r16.
* Nuke some logging.
* Misc Scheduler improvements.
* Minor USB PD fixes.
* Upstream WireGuard to `v1.0.20220627`.
* Reduce LZ4 memory usage to 16KB.
* Switch to LZ4 for pstore compression.
* Add support for last_kmsg.
* Build debugfs to keep userspace cutils sane.
* Expose Simple_LMK parameters to sysfs.
* Fix file append while using FUSE Passthrough.
* Backport a page_alloc patch in accordance to a previous backport.
* Kill UserLand Worker when flashed in an inline build.
* Enable Legacy QTI MSM RNG support.
* Add a timeout for some nasty power driver wakelocks.
* Grab MGLRU from android-4.14-stable gerrit.
* Add Simple_LMK hooks to MGLRU.
* Misc CFQ improvements.
* Linked with LLD 16.0.0.
* Deep Sleep of Death supposedly fixed.
