.. _hpcEnvironmentsOverview:

HPC Environments
================

Toil is a flexible framework that can be leveraged in a variety of environments, including high-performance computing (HPC) environments.
Toil provides support for a number of batch systems, including `Grid Engine`_, `Slurm`_, `Torque`_ and `LSF`_, which are popular schedulers used in these environments.
Toil also supports `HTCondor`_, which is a popular scheduler for high-throughput computing (HTC).
To use one of these batch systems specify the "-\\-batchSystem" argument to the toil script.

Due to the cost and complexity of maintaining support for these schedulers we currently consider them to be "community supported", that is the core development team does not regularly test or develop support for these systems. However, there are members of the Toil community currently deploying Toil in HPC environments and we welcome external contributions.

Developing the support of a new or existing batch system involves extending the abstract batch system class :class:`toil.batchSystems.abstractBatchSystem.AbstractBatchSystem`.

.. _Grid Engine: http://www.univa.com/oracle

.. _Slurm: https://www.schedmd.com/

.. _Torque: http://www.adaptivecomputing.com/products/open-source/torque/

.. _LSF: https://en.wikipedia.org/wiki/Platform_LSF

.. _HTCondor: https://research.cs.wisc.edu/htcondor/
