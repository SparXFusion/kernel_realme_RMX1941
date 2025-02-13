#
# Copyright (C) 2017 MediaTek Inc.
#
# This program is free software: you can redistribute it and/or modify
# it under the terms of the GNU General Public License version 2 as
# published by the Free Software Foundation.
#
# This program is distributed in the hope that it will be useful,
# but WITHOUT ANY WARRANTY; without even the implied warranty of
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
# GNU General Public License for more details.
#

#$(call all-subdir-src-or-makefile)
MTK_PLATFORM := $(subst ",,$(CONFIG_MTK_PLATFORM))
subdir-ccflags-y += -Werror
subdir-ccflags-$(CONFIG_MACH_MT6761) += -I$(srctree)/drivers/misc/mediatek/scp/mt6765

subdir-ccflags-y += -I$(srctree)/drivers/misc/mediatek/include
subdir-ccflags-y += -I$(srctree)/drivers/misc/mediatek/include/mt-plat/$(MTK_PLATFORM)/include
subdir-ccflags-y += -I$(srctree)/drivers/misc/mediatek/include/mt-plat/
subdir-ccflags-y += -I$(srctree)/drivers/mmc/host/mediatek/$(MTK_PLATFORM)

obj-$(CONFIG_MTK_EMI) += emi/
obj-$(CONFIG_MTK_EMI_BASIC) += emi/
obj-$(CONFIG_MTK_EMI_MPU) += emi_mpu/
obj-$(CONFIG_MTK_ICE_DEBUG) +=ice_debug/
obj-$(CONFIG_MTK_BASE_POWER) += base/

obj-$(CONFIG_MTK_ACCDET) += accdet/
obj-$(CONFIG_MEDIATEK_SOLUTION) += sched/
obj-$(CONFIG_MTK_FREQ_HOPPING) += freqhopping/
obj-$(CONFIG_MMC_MTK_SDIO) += mtk_sdio/
obj-$(CONFIG_MTK_COMBO) += connectivity/
obj-$(CONFIG_MTK_CONN_MD) += conn_md/
obj-$(CONFIG_MTK_BTIF) += btif/
obj-$(CONFIG_MTK_UNIFIED_DEBUG_INTERFACE) += udi/
obj-$(CONFIG_MTK_DEVAPC_DRIVER) += devapc/
obj-$(CONFIG_MTK_TRNG_DRIVER) += trng/
obj-$(CONFIG_MTK_MEM) += mem/
obj-$(CONFIG_MTK_MEMORY_LOWPOWER) += memory-lowpower/
obj-y += memory-amms/
obj-$(CONFIG_MTK_AUXADC)	+= auxadc/
obj-$(CONFIG_MTK_GPT_SCHEME_SUPPORT)	+= partition/
obj-$(CONFIG_MTK_SYSENV)	+= sysenv/
obj-$(CONFIG_MTK_PWM)	    += pwm/
obj-$(CONFIG_MTK_VIBRATOR)	+= vibrator/
obj-y += irtx/
obj-$(CONFIG_MTK_MT6306_GPIO_SUPPORT) += gpio/
obj-$(CONFIG_MTK_GIC_EXT) += ext_gic/
obj-$(CONFIG_MTPROF)	+= mtprof/
obj-$(CONFIG_MTK_PMIC_WRAP_HAL) += pmic_wrap/
obj-$(CONFIG_MTK_USBFSH) += usb11/
obj-$(CONFIG_USB_MTK_HDRC) += usb20/
obj-$(CONFIG_MTK_ECCCI_C2K) += c2k_usb/
obj-$(CONFIG_MTK_LEDS)	+= leds/
obj-$(CONFIG_MTK_BOOT) += boot/
obj-$(CONFIG_MTK_BOOT_REASON) += boot_reason/
obj-$(CONFIG_MTK_CHIP) += chip/
obj-$(CONFIG_MTK_SELINUX_AEE_WARNING)	+= selinux_warning/
obj-y += power/
obj-$(CONFIG_MTK_PMIC_NEW_ARCH)	+= pmic/
obj-$(CONFIG_MTK_AUDIODSP_SUPPORT) += adsp/
obj-$(CONFIG_MTK_AUDIODSP_SUPPORT) += audio_ipi/
### Please note that sensor must precede scp. ###
obj-$(CONFIG_MTK_SENSORS_1_0) += sensors-1.0/
obj-$(CONFIG_MTK_TINYSYS_SCP_SUPPORT) += scp/
obj-$(CONFIG_MTK_TINYSYS_SCP_SUPPORT) += audio_ipi/
obj-y += devinfo/
obj-$(CONFIG_MTK_GPU_SUPPORT) += gpu/
obj-$(CONFIG_MTK_LCM) += lcm/
obj-$(CONFIG_MTK_LCM) += ext_disp/
obj-$(CONFIG_MTK_SYNC) += sync/
obj-$(CONFIG_MTK_SECURITY_SW_SUPPORT) +=masp/
obj-$(CONFIG_MTK_BLOCK_TAG) +=blocktag/
obj-y += pidmap/
obj-$(CONFIG_MTK_KEY_HINT) += keyhint/
obj-$(CONFIG_MTK_IMGSENSOR) += imgsensor/src/
obj-$(CONFIG_MTK_CAM_CAL) += cam_cal/src/
ifneq ($(wildcard $(srctree)/drivers/misc/mediatek/met_drv/),)
obj-y += met_drv/
endif
obj-$(CONFIG_MTK_CCCI_DEVICES)	+=  ccci_util/
obj-$(CONFIG_MTK_MIX_DEVICES) +=  mixdev/
obj-$(CONFIG_MTK_NET_CCMNI) +=  ccmni/
obj-$(CONFIG_MTK_ECCCI_DRIVER) +=  eccci/
obj-$(CONFIG_TRUSTONIC_TEE_SUPPORT) += gcpu/
obj-$(CONFIG_MTK_IN_HOUSE_TEE_SUPPORT) += gcpu/
obj-$(CONFIG_MTK_IN_HOUSE_TEE_SUPPORT) += mtee/
ifeq ($(CONFIG_HAVE_MTK_IN_HOUSE_TEE_SUPPORT),y)
obj-$(CONFIG_TRUSTY) += gcpu/
endif
obj-$(CONFIG_TRUSTONIC_TEE_SUPPORT) += gud/
obj-$(CONFIG_MTK_TRUSTED_MEMORY_SUBSYSTEM) += trusted_mem/
obj-$(CONFIG_MTK_GZ_KREE) += geniezone/
obj-$(CONFIG_MTK_DEVMPU) += devmpu/
obj-y += sspm/
obj-$(CONFIG_MMPROFILE) += mmp/
obj-$(CONFIG_MTK_M4U)	+= m4u/
obj-$(CONFIG_MTK_PSEUDO_M4U)   += pseudo_m4u/
obj-$(CONFIG_MTK_SMI_EXT)	+= smi/
obj-$(CONFIG_MTK_USB_TYPEC) += typec/
obj-$(CONFIG_MTK_GPU_SUPPORT) += gpu/
obj-$(CONFIG_MTK_VPU_SUPPORT) += vpu/
obj-$(CONFIG_MTK_MDLA_SUPPORT) += mdla/
obj-$(CONFIG_MTK_CCU)	+= ccu/src/
obj-$(CONFIG_MTK_EDMC_SUPPORT) += edmc/
obj-$(CONFIG_MTK_RTC)	+= rtc/
obj-y += mtprintk/
obj-$(CONFIG_MTK_XO)	+= xo/
obj-$(CONFIG_MICROTRUST_TEE_SUPPORT) += teei/
obj-$(CONFIG_MTK_RAM_CONSOLE) += ram_console/
obj-$(CONFIG_MTK_DRAM_LOG_STORE)    += log_store/
obj-$(CONFIG_MEDIATEK_SOLUTION)	+= aee/
obj-$(CONFIG_MTK_MLOG) += mlog/
obj-$(CONFIG_MTK_CACHE_CONTROL) += cache-auditor/
obj-y += cameraisp/
obj-$(CONFIG_MTK_CMDQ) += cmdq/
obj-$(CONFIG_MTK_CMDQ) += mdp/
obj-$(CONFIG_MTK_CMDQ_TAB) += cmdq/
obj-$(CONFIG_MTK_CQDMA) += cqdma/
obj-$(CONFIG_MTK_LCM) += lcm/
obj-$(CONFIG_MTK_LCM) += ext_disp/
obj-$(CONFIG_MTK_HDMI_SUPPORT) += hdmi/
obj-$(CONFIG_MTK_FB) += video/
obj-$(CONFIG_MTK_DYNAMIC_FPS_FRAMEWORK_SUPPORT) += dfrc/
obj-$(CONFIG_MTK_SYNC) += sync/
obj-$(CONFIG_MTK_LENS)   += lens/
obj-$(CONFIG_MTK_FLASHLIGHT) += flashlight/
obj-$(CONFIG_RT_FLASHLIGHT)     += flashlight/richtek/
obj-$(CONFIG_RT_REGMAP) += rt-regmap/
obj-$(CONFIG_MTK_VIDEOCODEC_DRIVER) += videocodec/
obj-$(CONFIG_MTK_JPEG)	+= jpeg/
obj-$(CONFIG_MD32_SUPPORT)     += md32/
obj-$(CONFIG_USB)	+= usb_boost/
obj-$(CONFIG_MU3_PHY)   += mu3phy/
obj-$(CONFIG_USB_MU3D_DRV)	+= mu3d/
obj-$(CONFIG_MTK_SMARTPA_SOUND)	+= smartpa/
obj-$(CONFIG_MTK_SYS_CIRQ) += cirq/
obj-y += atf/
obj-$(CONFIG_THERMAL)   += thermal/
obj-$(CONFIG_MTK_SSMR) += memory-ssmr/
obj-$(CONFIG_ZONE_MOVABLE_CMA) += zone_movable_cma/
obj-$(CONFIG_MTK_DEBUG_LATCH)   += debug_latch/
obj-$(CONFIG_MTK_DFD_INTERNAL_DUMP) += dfd/
obj-$(CONFIG_MTK_SYSTRACKER)   += systracker/
obj-$(CONFIG_MEDIATEK_SOLUTION) += cmo/
obj-$(CONFIG_MTK_VOW_SUPPORT)  += vow/
ifneq (, (filter y,$(CONFIG_MTK_MD_DIRECT_TETHERING_SUPPORT) $(CONFIG_MTK_MDDP_WH_SUPPORT) $(CONFIG_MTK_MCIF_WSVC_SUPPORT)))
obj-y += mddp/
endif
obj-y += timer/
obj-$(CONFIG_NFC_CHIP_SUPPORT) += nfc/
obj-$(CONFIG_MTK_DRAMC) += dramc/
obj-y += performance/
obj-$(CONFIG_MTK_FIQ_CACHE) += fiq_cache/
obj-$(CONFIG_MTK_DEBUG_LATCH) += debug_latch/
obj-$(CONFIG_MTK_USB2JTAG_SUPPORT) += usb2jtag/
obj-$(CONFIG_MTK_WATCHPOINT) += watchpoint/

obj-$(CONFIG_TRUSTKERNEL_TEE_SUPPORT) += tkcore/
obj-$(CONFIG_MTK_PERF_TRACKER) += perf/

#io boost
obj-y += io_boost/
