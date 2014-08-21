SDN-OpenFlowRecovery
====================

Contains patches to Open vSwitch for our paper "Fast Recovery in Software-Defined Networks"

The folder src contains a fully pre-patched Open vSwitch.
The original source as pulled from http://openvswitch.org/cgi-bin/gitweb.cgi?p=openvswitch;a=snapshot;sf=tgz;h=HEAD at 10th of April 2014 (filename and commit openvswitch-HEAD-50c1efc.tar.gz).  

The file OpenFlowRecovery.patch contains the patch file made using `git diff --no-prefix` and can be used to patch the source-code by oneself.

