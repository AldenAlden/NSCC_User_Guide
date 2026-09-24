# System Specifications

## Compute Nodes
| Type | # Nodes | Per Node<br><br>CPU | <br><br>GPU | <br><br>RAM | <br><br>Storage | PBS Queue
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Cray EX CPU Nodes | 768 | 2 x [AMD EPYC™ 9655](https://www.amd.com/en/products/processors/server/epyc/9005-series/amd-epyc-9655.html)<br>96 cores per CPU<br>192 cores in total | - | 770GB DDR5 ECC | - | normal |
| Cray EX GPU Nodes | 192 | 2 x [AMD EPYC™ 9655](https://www.amd.com/en/products/processors/server/epyc/9005-series/amd-epyc-9655.html)<br>96 cores per CPU<br>192 cores in total | 8 x [NVIDIA H200 Tensor Core GPU](https://www.nvidia.com/en-sg/data-center/h200/) | 2.3TB DDR5 ECC | - | normal |
| Large Memory Nodes | 16 | 2 x [AMD EPYC™ 9554](https://www.amd.com/en/products/processors/server/epyc/4th-generation-9004-and-8004-series/amd-epyc-9554.html)<br>64 cores per CPU<br>128 cores in total | - | 4TB DDR5 ECC | 30TB Micron NVMe SSD | normal |

## Network
- Slingshot 400 interconnect
- Dragonfly Plus topology
- 400 Gbps PCIe Gen5 NICs

## Storage
> [!WARNING]
> All data on NSCC systems is governed by the [Data Management and Retention Policy](https://nsccsg.github.io/policies/data-management-and-retention-policy/). Read it carefully to **prevent data loss, maintain proper access, and manage your data securely.**

| Directory | Filesystem | Capacity | Mount Point | Quota | Use Case |
| :--- | :--- | :--- | :--- | :--- | :--- |
| Home | LFS | 2.3PB | ```/home/users/<org>/<institution>/<username>/``` | 50GB | Long term storage of user data |
| Project | LFS | 35PB | ```/project/<project-id>/``` | Project specific | Long term storage of project data shared among members |
| Scratch | LFS | 23PB | ```/scratch/users/<org>/<institution>/<username>/``` | 100TB | Temporary storage of user data for better I/O performance(subject to purge) |
