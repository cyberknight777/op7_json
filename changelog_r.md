## Build Information
```
Kernel: DragonHeart Kernel
Type: Bleeding Edge
Device: OnePlus 7/T/P
Compiler: Eva GCC 12.1.1
Branch: staging
Build Number: r16b3-hotfix
```
## Changelog
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
