# base data

## relevant from reco log

dtb index 13
dtbo index 47
boot device 1d840000.ufshc
verity enforce
usbcontroller a600000.dwc3
test-keys???
vbmeta 11712

## Partition sizes

* Recovery image partition size matches ( 0x6400000 == 104857600 )
* Vendor sizes match ( 0x6000000 == 100663296 )
* Boot sizes match  ( 0x6000000 == 100663296 )
* re: dtb / dtbo partition sizes
  * 25165824 is the size here times 2. Not sure if that's relevant?

## cmdline
stack_depot_disable=on kasan.stacktrace=off kvm-arm.mode=protected cgroup_disable=pressure cgroup.memory=nokmem console=ttyMSM0,115200n8 loglevel=6 log_buf_len=256K kernel.panic_on_rcu_stall=1 loop.max_part=7 pcie_ports=compat msm_rtb.filter=0x237 kasan=off rcupdate.rcu_expedited=1 rcu_nocbs=0-7 ftrace_dump_on_oops pstore.compress=none kpti=0 swiotlb=noforce cgroup.memory=nokmem,nosocket kswapd_per_node=2 slub_debug=- allow_file_spec_access cpufreq.default_governor=performance transparent_hugepage=never can.stats_timer=0 disable_dma32=on android12_only.will_be_removed_soon.memblock_nomap_remove=on pcie_ports=compat video=vfb:640x400,bpp=32,memsize=3072000 bootconfig buildvariant=user  msm_drm.dsi_display0=qcom,mdss_dsi_ft7131m_1080p_video: rootwait ro init=/init silent_boot.mode=nonsilent

## edid extract

Used: https://askubuntu.com/questions/81370/how-to-create-extract-the-edid-for-from-a-monitor

Found: /sys/class/drm -> card0-DSI-1 has edid