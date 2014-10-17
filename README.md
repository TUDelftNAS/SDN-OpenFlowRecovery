SDN-OpenFlowRecovery
====================

This repository contains the sourcecode of, and patches to Open vSwitch to perform the experiments in our paper "Fast Recovery in Software-Defined Networks" as appearing in the proceedings of the Third European Workshop on Software Defined Networking (EWSDN), Budapest, Hungary, September 1-3

When you use this work for academical or educational references, please cite the paper instead of this repository.
BibTeX:
@inproceedings{vanadrichemopenflowrecovery,
  title={Fast Recovery in Software-Defined Networks},
  author={van Adrichem, Niels L. M. and van Asten, Benjamin J. and Kuipers, Fernando A.},
  booktitle={Software Defined Networks (EWSDN), 2014 Third European Workshop on},
  year={2014},
  organization={IEEE}
}

The folder src contains a fully pre-patched Open vSwitch.
Being, the original source as pulled from http://openvswitch.org/cgi-bin/gitweb.cgi?p=openvswitch;a=snapshot;sf=tgz;h=HEAD at 10th of April 2014 (filename and commit openvswitch-HEAD-50c1efc.tar.gz) with the necessary adaptations to perform our measurements.  

The file OpenFlowRecovery.patch contains the patch file made using `git diff --no-prefix` and can be used to patch the source-code by oneself.

As of 17 october 2014, BFD support in Open vSwitch has been integrated into the FastFailover Group Tables, hence, for operational purposes this patch is not necessary anymore. Until release into the stable branch you can clone from the Open vSwitch GitHub repository However, the measurements in the mentioned paper may not be representable for this implementation due to implementational differences in the code.
