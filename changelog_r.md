## Build Information
```
Kernel: DragonHeart Kernel
Type: Bleeding Edge
Device: OnePlus 7/T/P
Compiler: Eva GCC 12.2.1
Branch: staging
Build Number: r16b8
```
## Changelog
**-r16b8**
* Upgrade ZSTD to latest upstream v1.5.4.
* Add per-cpu threads for decompression in EROFS for better app launches and boot time.
* Set scheduler to use SCHED_RR at high priority for lower latency.
* Drop deprecated check for A12 ROMs
* FOD optimizations from John.
* Inline FP/TS drivers.
* Re-add display partial updates.
* Correct 60hz fod down timing.
* Decrease min brightness on AOD.
* Misc optimizations.

**-r16b7**
* Grab new CSC DC Dim implementation.
* Implement new double tap attr for modernized DT2W.
* Kill legacy double tap impl.
* In-kernel handling for random crashy 7T adsp.
* Import tuned dim lut for all variants.
* Simplify double_tap_pressed handling

**-r16b6**

* Grab all recent FOD improvements from John.
* Update in-kernel LZ4 to v1.9.4
* Fix crashdumps for ESOC devices permanently.
* Increase rating of teo governor to 50.
* Save power when connecting to an USB.
* Disable QCOM download mode.
* Prevent kernel panic caused by adsp crash.

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
