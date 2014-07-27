obj-m += i2c-designware-core.o
obj-m += i2c-designware-platform.o
i2c-designware-platform-objs := i2c-designware-platdrv.o
obj-m += i2c-designware-pci.o
i2c-designware-pci-objs := i2c-designware-pcidrv.o

KDIR := /lib/modules/$(shell uname -r)/build
PWD := $(shell pwd)

all:
	$(MAKE) -C $(KDIR) M=$(PWD) modules

clean:
	$(MAKE) -C $(KDIR) M=$(PWD) clean
