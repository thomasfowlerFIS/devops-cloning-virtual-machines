# **Cloning Virtual Machines in VirtualBox**

Course: DevOps

Mod: Week 1

Topic: Cloning Virtual Machines in VirtualBox

Amount of time: 1.5 hours

Author: Thomas Fowler

## **Lesson Objectives**

* Describe what cloning a virtual machine does.

* Understand the differences between clone types.

* Identify important configuration choices when cloning virtual machines.

--------------------------------------------

### **Cloning a Virtual Machine in VirtualBox**

In earlier lessons, virtualization is described as emulating a physical
machine in software. Since a virtual machine is software-based, they
have the inherent capability of being replicated or cloned. The clone
from a virtual machine is virtually identical in every way, except for
some implementation-specific or user-defined settings when cloning.

This means that once a virtual machine is provisioned and configured to
a user's specification, it can be cloned and reprovisioned again as
its own unique instance. This can also include uniqueness at the
hardware level. For instance, the cloned virtual machine can have its
own unique MAC address on its network adapter(s). As a result, if a
virtual machine is cloned three times, each having its own unique MAC
address, from a networking perspective each clone appears as a separate
physical machine on the network.

### **Clone Types**

When cloning a virtual machine in Virtual Box there are two types to select
from: a full clone or a linked clone. Full clones are exact copies of the
original or source virtual machine, with the exception that their storage
volumes are unique. Linked clones on the otherhand are exact copies of the
source VM, except they share the same storage volume.

--------------------------------------------

#### **Full Clone**

Not only do full clones use their own independent disk images, they also
copy _all_ disk dependencies from the source. Full clones can operate
completely independently of the source VM and include all previous
snapshots of the source VM before the source VM's current state.

--------------------------------------------

#### **Linked Clone**

When cloning a VM as a linked clone, the cloned VM shares the source VM's
disk image. This clone type is typical given the lack of extra disk usage
on the host machine's storage. While this is typically beneficial keeping
the host disk's usage down, as the number of clones sharing the same
virtual disk image increases, the faster the rate at which the shared
disk image's capacity diminishes.

--------------------------------------------

### **Considerations for Different Clone Types**

When cloning virtual machines in VirtualBox, an option exists to generate
new MAC Addresses for the clone's network adapters. This is suitable for
most scenarios, as _not_ generating new MAC addresses for a clone's
network adapters would make it appear as another machine on the network.

