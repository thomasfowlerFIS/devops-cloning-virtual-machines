# **Cloning Virtual Machines in Virtual Box**

Course: DevOps

Mod: Week 1

Topic: Cloning Virtual Machines

Amount of time: 1.5 hours

Author: Thomas Fowler

## **Lesson Objectives**

* Describe what cloning a virtual machine does.

* Understand the differences between clone types.

* Identify important configuration choices when cloning virtual machines.

--------------------------------------------

### **Cloning a Virtual Machine**

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

When cloning a virtual machine in Virtual Box

#### **Full Clone**

#### **Linked Clone**

--------------------------------------------

### **Considerations for Different Clone Types**

--------------------------------------------
