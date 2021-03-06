# Roadmap & Accomplishments

_The below "timeline" is a rough outline on when we can expect different milestones to be accomplished - the order does not reflect their relative priorities or the amount of effort spent_.


## In progress

* Expansion: Migrate QB3 users and QB3 compute nodes (7,000 physical cores) over to Wynton HPC (approximately 1,500 out of 7,000 cores still to be migrated - September 2019)


## Soon

* ...


## Near future

* Pricing model: Contributors to Wynton get access to a larger compute share of the cluster (beyond what is available for free).  Details on how to contribute with new hardware (amount in USD) and how to contribute with existing hardware (minimum technical requirements) will be given

* Storage: Requirements for mounting lab-owned storage into Wynton

* Forum: A self-hosted User Forum for richer conversations than what's on our Slack channel

* Scheduler: Slurm as a job scheduler instead of SGE

## On the horizon

* Support: A User Issue Tracker

* Compliance: Support for restricted data analysis

* Network: Add a Globus endpoint for efficient, secure data transfers (ingress and egress)



## Accomplished milestones

* Migration: The UCSF Memory and Aging Center (MAC) have joined Wynton by contributing new nodes

* Migration: The UCSF Macromolecular Structure Group (MSG) compute cluster (~1,300 physical cores) is incorporated into Wynton

* Development: Dedicated 10 Gbps transfer node for faster file transfers in to and out from Wynton (2018-08-02)

* Storage: Global scratch storage on BeeGFS parallel file system (2018-08-20)

* Pricing model: Description on how to purchase (amount in USD) additional storage space beyond what is available for free (2019-01-15)

* Development: Additional development nodes for building software to take load off the current development node (2019-01-31)

* GPU compute: Four communal GPU nodes with a total of 12 GPUs from the QB3 cluster (2019-04-12)

* Development: A dedicated Graphics Processing Unit (GPU) development node for building GPU software (2019-04-15)

* Software stacks: Support for sharing software installations between groups via environment modules, e.g. `module load CBI` (2019-06-13)

* Storage: The QB3-legacy NetApp scratch storage `/scrapp` and `/scrapp2` has been removed in favor of the BeeGFS-based scratch storage `/wynton/scratch` (2019-08-15)

* Scheduler: ~~Support interactive jobs (`qlogin`)~~. The Wynton HPC Team decided against this because it increases the risk of having stale jobs occupying the scheduler and overall underutilizing the HPC environment (Fall 2019)

* Development: A second data transfer node for faster file transfers in to and out from Wynton (2019-09-12)

* GPU compute: An additional 12 communal GPUs on three GPU nodes (2019-09-13)

* GPU policy: All GPU nodes, communal and contributed, are available to all users. When running on another contributors GPU node, run time is limited to 2 hours. (2019-09-20)

* Scheduler: Support for email notification upon job completion, e.g. `qsub -m bea` (2019-11-12)

* Storage: The QB3-legacy NetApp storage (including `/netapp/home`) was deprecated during 2019 with a deadline on December 2019.  The server was kept up after this deadline and, unfortunately, the server went down on 2020-02-05 and was declared non-recoverable without further resource/funding (2020-02-05)

* Storage: Migrate home directories from the NetApp server (`/netapp/home/`) to the new, faster BeeGFS parallel file system (`/wynton/home/`).  The migration effort ended on 2020-02-05 when the NetApp server failed (2020-02-05)

* Website: Move website from GitHub Pages (https://ucsf-hpc.github.io/wynton/) with on-premise https://wynton.ucsf.edu/hpc/


See also [News].



[QB3]: https://salilab.org/qb3cluster/
[BeeGFS]: https://www.beegfs.io/
[Globus]: https://www.globus.org/
[News]: {{ '/about/news.html' | relative_url }}
