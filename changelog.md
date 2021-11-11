## Build Information
```
Kernel: DragonHeart Kernel
Type: Stable
Device: OnePlus 7/T/P
Compiler: Eva GCC 12.0.0
Branch: master
Build Number: rc1
```
## Changelog
**-rc1**

* rebased off LA.UM.9.1.r1-11300-SMxxx0.0
* imported wlan and techpack off LA.UM.9.1.r1-11300-SMxxx0.0
* build rmnet extensions
* switch to power_efficient workingqueue for techpack
* optimize techpack for size and nuke debug information on it
* reduce debugging in qcacld
* optimize qcacld for size and nuke debug information on it
* switch to power efficient workingqueue for qca-wifi-host-cmn
* upstreamed dtc to v1.4.6-9
* added z order fod commit
* added cpuidle patches and backports for better deep sleep
* added -pipes optimization
* nuked trace_printk()
* switched to -O3 treewide
* switched to -O3 for LLD
* optimized flags for kryo 485
* optimized for crypto and crc
* optimized arch specfic code for kryo 485, crypto and crc
* nuke auditing
* enabled store motion pass for global common subexpression elimination(GCSE)
* imported wireguard  v1.0.20210606
* enabled TTL & HL fixations
* picked gulch's treewide/oneplus: massive code removal commit
* cleaned up unneeded synaptic drivers
* inlined i2c interfaces for touch drivers
* disable auto test for s3706 driver
* conditionally compile out auto_test functions
* enforce msm drm notifier for touch drivers
* nuke logging in touch driver
* init touch drivers earlier
* imported vDSO32
* switched to -O3 for vDSO32
* picked masahiro's kbuild commits for quality of life
* enabled lse_atomics
* inlined spinlocks
* enabled DCE
* picked fp inlining commits for faster fp
* enforce msm drm notifier for fp
* enabled OPTIMIZE_INLINING
* picked power efficient workingqueues treewide
* picked & enabled BBR
* switched to WESTWOOD for default tcp congestion algorithm
* imported srandom
* switched to srandom over hw_random
* backported cgroup commits
* nuked debugging configs
* upstreamed lz4
* switched to lz4 as default crypto compression algorithm
* switched to zswap over zram
* used vbswap as a fake block device for zswap
* nuke additional ext4 tracing by caf
* add haptic level adjustment
* drop samsung_oneplus_dsc 1080p timings to fix google maps
* introduced tri-cluster api to affine IRQs
* introduced cpumasks for big, LITTLE and prime cpu masks
* affined IRQs treewide
* introduced sched api to migrate current process to a given cpumask
* Improved the scheduler and its mechanism(walt) by grabbing patches from CAF & RenderBroken
* checkout sched/energy to android-4.14-stable to move way from caf's mess
* introduced devfreq_boost to boost DDR bus on custom events
* affined hwcomposter to big CPUs
* imported simple_lmk and tune it for our needs
* disable CONFIG_DEBUG_KERNEL for lesser debugging
* introduce f2fs rapid gc 
* introduce cpu_input_boost to boost CPU on custom events
* speed up mremap by 20x 
* reduce time taken to enter sleep
* nuked more debugging and tracing
* switched to cfq as default iosched
* reduced devfreq wake boost duration to 500ms
* introduce kprofiles 1.0.0
* inline active_mode() for faster execution for kprofiles
* switch to case statement over if/else to reduce latency for kprofiles
* misc improvement to kprofiles codebase
* implement display notifiers for auto kprofiles
* bump kprofiles to 2.0.0
* take mode=0 into account for active_mode() for kprofiles
* introduce 2 new api for changing modes on custom events for kprofiles
* nuke redundant break statement in kprofiles
* export sysfs to allow user to disable auto kprofiles
* bump kprofiles to 3.0.0
* mark more kprofiles functions as inline
* refactor common notifier of kprofiles to use the new API
* rename mode 0 of kprofiles to normal for clarity
* fix build when AUTO_KPROFILES is disabled
* hardcode battery mode as default
* boost DDR bus and CPU according to profile set for zygote forking (app launches)
* boost DDR bus and CPU according to profile set for frame rendering (smoothness)
* force set freqs to max/min depending on profile set for performance governor
* increase gpu data processing limit
* forbid init from changing iosched
* introduce STREEBOG algorithm for crypto operations
* reduce logging treewide
* reduce logging in binder
* silence log spam when cpu is brought up
* skip OOM_KILLER when compiled for android
* nuke rmnet logging
* disable NL80211_TESTMODE
* use TCP_NODELAY to improve network latency
* use an efficient frequency table with an optimized energy model
* configured minimum idle frequency for better idle drain
* confugured min freq fallback after boosting for better overall drains
* switch to 50hz kernel tickrate
* force gpu idle timeout to 58ms
* implement rhel's low latency cmdline for less latency
* power off dsi phy during idle to save more power
* remove pm qos active latency override
* nuke display ramdump mem region
* nuke unused 36 MiB memdump region for less ram usage
* disable broken IRQ detection
* enable freq-energy-model to correlate with checkout of sched/energy to android-4.14-stable
* add new GPU step from CAF
* enable some panel tweaks for oneplus displays
* cleanup dtbo building
* suppress verbose output for cmdline
* configure frame transfer time to 800us
* misc improvements to dtsi
* spoof fake kernel version to fsck
* mm patches from sultan for overall improvement of mm
* nuke pm qos implementation in adsp to save power
* enable RELR relocation packing for smaller image
* compile out ipa_v3 wakelock code
* add timeout to wakelocks globally
* nuke pm qos usage in vidc for less power used during media playback
* fix misconfigured irq in rpmsg
* revert logging of interrupts for GICv3
* built with EvaGCC 12.0.0
* used LLD 13.0.0 as linker
