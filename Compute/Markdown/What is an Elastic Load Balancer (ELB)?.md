Distributes inbound requests evenly across the target resource group. The group could be a fleet of EC2 instances, a range of IP addresses or Containers.

Targets can be defined across different Azs or all placed in one AZ.

## ELB Example
You have created a new app and it is running on a single EC2 instance. It is being accessed by a number of users. Your architecture might initially look like this:

![[ELB Example 1]]

This means that if the single instance fails, your application will be down. The instance may also be unable to handlethe increased load of spikes in traffic.

Adding an ELB to distribute traffic across multiple instances avoids these problems:

![[ELB Example 2]]

ELB is highly available because it is a managed service.

If any instances fail, the ELB will automatically detect and divert. The additional instances help with the load where there is a surge in traffic.

![[ELB Example 3]]

The ELB dynamically scales up and down as needed.

There are three ELBs to choose from: