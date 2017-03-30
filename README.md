# bug_report_libvirt
Bug#841291

Bug is the following

~~~
error: internal error: process exited while connecting to monitor: 2017-03-30T08:57:59.661143Z qemu-system-x86_64: -drive if=none,id=drive-ide0-0-1,readonly=on,format=raw: Can't use 'raw' as a block driver for the protocol level
~~~

# setup

to reproduce the bug, you need Vagrant and Virtualbox

~~~
vagrant up
vagrant ssh
virsh -c qemu:///system start test_vm
~~~
