ccflags-y := $(INCDIR)

obj-m	+= nvmet.o
obj-m	+= nvme-loop.o
obj-m	+= nvmet-rdma.o
obj-m	+= nvmet-fc.o
obj-m	+= nvme-fcloop.o
obj-m	+= nvmet-tcp.o
obj-m	+= i10-target.o

nvmet-objs			+= core.o configfs.o admin-cmd.o fabrics-cmd.o discovery.o io-cmd-file.o io-cmd-bdev.o
nvme-loop-objs		+= loop.o
nvmet-rdma-objs		+= rdma.o
nvmet-fc-objs		+= fc.o
nvme-fcloop-objs	+= fcloop.o
nvmet-tcp-objs		+= tcp.o
i10-target-objs		+= i10.o
