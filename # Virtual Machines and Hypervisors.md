# Virtual Machines and Hypervisors

## 1. What Is a Virtual Machine?

A **Virtual Machine (VM)** is a software-based computer that runs inside a physical computer.

It behaves like a real computer and can have:

- Virtual CPU
- Virtual RAM
- Virtual storage
- Virtual network
- Operating system
- Applications

A VM uses the resources of a physical computer but works as an independent computer.

## 2. Simple Real-World Example

Imagine that you have one powerful physical computer.

Instead of using it to run only one operating system, you create three virtual machines:

- VM 1: Windows
- VM 2: Ubuntu Linux
- VM 3: Another Linux system

Now, one physical computer can run multiple operating systems at the same time.

Each virtual machine behaves like a separate computer.

## 3. Physical Machine vs Virtual Machine

### Physical Machine

A physical machine is an actual computer or server that contains hardware such as:

- CPU
- RAM
- Hard disk or SSD
- Network card
- Motherboard

### Virtual Machine

A virtual machine is created using software.

It uses a portion of the physical machine's resources, such as:

- Virtual CPU
- Virtual RAM
- Virtual disk
- Virtual network

A VM does not normally require a separate physical computer.

## 4. Why Are Virtual Machines Needed?

### 4.1 Better Resource Utilization

A powerful physical server may not use all of its resources.

Virtual machines allow multiple workloads to run on the same physical server.

### 4.2 Cost Reduction

Instead of purchasing separate physical servers for every application, multiple VMs can run on one physical server.

This can reduce hardware and maintenance costs.

### 4.3 Isolation

Each VM works in an isolated environment.

If one VM experiences a problem, other VMs may continue working, depending on the type of failure.

### 4.4 Running Multiple Operating Systems

A single physical computer can run multiple operating systems through virtual machines.

For example:

- Windows
- Ubuntu
- Fedora

### 4.5 Easy Management

Virtual machines can be created, deleted, copied, backed up, and managed using software.

## 5. What Is a Hypervisor?

A **Hypervisor** is software, firmware, or a combination of software and hardware that creates and manages virtual machines.

It manages the physical computer's resources and distributes them among different virtual machines.

The hypervisor controls resources such as:

- CPU
- RAM
- Storage
- Network

## 6. How Does a Hypervisor Work?

The hypervisor is placed between the physical hardware and virtual machines.

It allocates physical resources to each virtual machine.

### Basic Structure

Physical Hardware
       |
       v
   Hypervisor
       |
       +----------------+
       |                |
       v                v
     VM 1             VM 2
   Windows           Linux

The hypervisor makes it possible for multiple VMs to share the same physical hardware.

## 7. Types of Hypervisors

There are two main types of hypervisors:

1. Type 1 Hypervisor
2. Type 2 Hypervisor

## 8. Type 1 Hypervisor

A **Type 1 hypervisor** runs directly on the physical hardware.

It does not require a traditional host operating system underneath it.

It is also called a **bare-metal hypervisor**.

### Structure

Physical Hardware
       |
       v
 Type 1 Hypervisor
       |
       +----------------+
       |                |
       v                v
     VM 1             VM 2

### Examples

- VMware ESXi
- Microsoft Hyper-V
- Xen

### Common Usage

Type 1 hypervisors are commonly used in:

- Data centers
- Enterprise servers
- Cloud infrastructure

## 9. Type 2 Hypervisor

A **Type 2 hypervisor** runs on top of an existing operating system.

The existing operating system is called the host operating system.

### Structure

Physical Hardware
       |
       v
 Host Operating System
       |
       v
 Type 2 Hypervisor
       |
       +----------------+
       |                |
       v                v
     VM 1             VM 2

### Examples

- Oracle VirtualBox
- VMware Workstation
- Parallels Desktop

### Common Usage

Type 2 hypervisors are commonly used for:

- Learning
- Testing
- Software development
- Running Linux on a Windows computer

## 10. Type 1 vs Type 2 Hypervisor

| Feature | Type 1 | Type 2 |
|---|---|---|
| Runs on | Physical hardware | Host operating system |
| Other name | Bare-metal | Hosted |
| Common usage | Data centers and servers | Personal computers and testing |
| Performance | Usually more direct | Has an additional host OS layer |
| Example | VMware ESXi | VirtualBox |

## 11. Important Terms

### Host Machine

The physical computer on which virtual machines run.

### Guest Machine

The virtual machine running inside the host machine.

### Host Operating System

The operating system installed on the physical computer.

This is mainly associated with Type 2 hypervisors.

### Guest Operating System

The operating system installed inside a virtual machine.

### Virtual Resources

The CPU, RAM, storage, and network resources assigned to a virtual machine.

## 12. How a VM Uses Physical Resources

Suppose a physical server has:

- 16 CPU cores
- 64 GB RAM
- 1 TB storage

The hypervisor can allocate resources to different virtual machines.

Example:

| Resource | VM 1 | VM 2 | VM 3 |
|---|---:|---:|---:|
| CPU | 4 cores | 4 cores | 2 cores |
| RAM | 16 GB | 16 GB | 8 GB |
| Storage | 200 GB | 200 GB | 100 GB |

The remaining resources can be reserved for other workloads or system operations.

The exact allocation depends on the hypervisor and configuration.

## 13. Virtual Machines and AWS

Cloud providers use physical data centers containing physical servers.

Virtualization technology allows cloud providers to divide physical resources into virtual servers.

In AWS, an **Amazon EC2 instance** is a virtual server that can be used to run applications.

A simplified relationship is:

Physical Server
       |
       v
 Virtualization
       |
       v
 Virtual Server
       |
       v
 EC2 Instance

An EC2 instance is not necessarily the same as manually creating a VM using VirtualBox on a personal computer, but both involve the concept of virtualized computing resources.

## 14. Virtual Machine vs Container

### Virtual Machine

- Includes a complete guest operating system
- Provides stronger isolation in many configurations
- Usually consumes more resources
- Can run a different operating system from the host

### Container

- Shares the host operating system kernel
- Packages an application and its dependencies
- Usually starts faster than a VM
- Generally uses fewer resources

Containers and virtual machines can also be used together.

## 15. Advantages of Virtual Machines

- Better utilization of physical resources
- Reduced hardware requirements
- Isolation between workloads
- Support for multiple operating systems
- Easy testing and development
- Easier backup and migration
- Useful for cloud infrastructure

## 16. Limitations of Virtual Machines

- Consume physical resources
- Require proper resource allocation
- Multiple VMs may compete for resources
- Performance depends on hardware and configuration
- A physical host failure may affect multiple VMs running on it

## 17. Key Points to Remember

1. A VM is a software-based computer.
2. A VM runs using resources from a physical machine.
3. A hypervisor creates and manages virtual machines.
4. Type 1 hypervisors run directly on physical hardware.
5. Type 2 hypervisors run on top of a host operating system.
6. Multiple VMs can run on one physical server.
7. Virtualization is an important foundation of cloud infrastructure.
8. EC2 provides virtual servers in AWS.

## 18. Quick Revision

### What is a VM?

A software-based computer that runs inside a physical computer.

### What is a hypervisor?

Software or firmware that creates and manages virtual machines.

### What is a Type 1 hypervisor?

A hypervisor that runs directly on physical hardware.

### What is a Type 2 hypervisor?

A hypervisor that runs on top of an existing operating system.

### Why are VMs used?

To improve resource utilization, reduce costs, provide isolation, and run multiple operating systems.

## 19. Doubts and Clarifications

This section will be updated whenever I ask questions during my learning journey.

### Doubt 1

**Question:** 

**Easy Explanation:** 

**Real-World Example:** 

**Key Point:** 

---