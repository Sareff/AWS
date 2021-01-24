202101201735
Tags: #z #aws #lessons 

---
# Spot Fleets 

Spot Fleet = set of Spot Instances + (optional) On-Demand Instances.

The Spot Fleet will try to meet the target capacity with price constraints. All you have to do is define possible launch pools (instance type, OS, [Availability Zone](<Availability Zones>)). You can have multiple launch pools, so that the fleet can choose. Spot Fleet stop launching instances when reaching capacity or max cost.

There are three strategies to allocate Spot Instances – lowest price, where spot fleet choose from the lowest price pool; diversified, where spot fleet distribute instances between all pools; and capacity optimized, where spot fleet choose pool with the optimal capacity for the number of instances

Spot Fleets allow you to automatically request Spot Instances with the lowest price.

---
### Zero-Links
- 
---
### Links
- [[EC2]]
- [[Launch type]]