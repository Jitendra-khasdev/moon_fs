PROG = moonfs
obj-m += ${PROG}.o                                                             
moonfs-objs := super.o inode.o file.o                              
                                                                                
all:                                                                            
	$(MAKE) -C /lib/modules/$(shell uname -r)/build/ M=$(shell pwd) modules       
clean:                                                                          
	$(MAKE) -C /lib/modules/$(shell uname -r)/build/ M=$(shell pwd) clean 
