ifdef CONFIG_INLINE_OPTIMIZATION
ccflags-y += -mllvm -inline-threshold=15000
ccflags-y += -mllvm -inlinehint-threshold=10000
endif

ccflags-y := -O3

ccflags-y += -I$(src)			# needed for trace events

obj-y					+= ion/

obj-$(CONFIG_ASHMEM)			+= ashmem.o
obj-$(CONFIG_ANDROID_VSOC)		+= vsoc.o
obj-$(CONFIG_ANDROID_INTF_ALARM_DEV)	+= alarm-dev.o
