ccflags-y := $(INCDIR)

obj-m		+= nvme-core.o
obj-m		+= nvme.o
obj-m		+= nvme-fabrics.o
obj-m		+= nvme-rdma.o
obj-m		+= nvme-fc.o
obj-m		+= nvme-tcp.o
obj-m		+= i10-host.o

nvme-core-objs	:= core.o
nvme-core-objs	+= trace.o
nvme-core-objs	+= multipath.o
#nvme-core-objs	+= lightnvm.o
#nvme-core-objs	+= fault_inject.o

nvme-objs			+= pci.o
nvme-fabrics-objs	+= fabrics.o
nvme-rdma-objs		+= rdma.o
nvme-fc-objs		+= fc.o
nvme-tcp-objs		+= tcp.o
i10-host-objs		+= i10.o