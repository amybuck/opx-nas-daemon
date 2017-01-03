# opx-nas-daemon
This repository contains the network abstraction service (NAS) daemon. This initializes the various components of NAS, and provides the process context for all NAS components (such as NAS L2 and NAS l3).

## Build
See [opx-nas-manifest](https://github.com/open-switch/opx-nas-manifest) for more information on common build tools.

### Build requirements

- `opx-base-model`
- `opx-common-utils`
- `opx-nas-common`
- `opx-object-library`
- `opx-logging`
- `opx-nas-ndi`
- `opx-nas-ndi-api`
- `opx-nas-linux`
- `opx-nas-interface`
- `opx-nas-l2`
- `opx-nas-l3`
- `opx-nas-platform-s6000`
- `opx-nas-acl`
- `opx-nas-qos`

Copy the Debian files to the parent folder (default location of Debian files), then run the `opx-build` command.

Dependent packages:  libopx-logging1 libopx-logging-dev libopx-common1 libopx-common-dev libopx-model1 libopx-model-dev libopx-object-library1 libopx-object-library-dev libopx-nas-common1 libopx-nas-common-dev opx-ndi-api-dev opx-sai-api-dev libopx-nas-ndi1 opx-object-library opx-nas-ndi-api-dev libopx-nas-ndi-dev libopx-nas-linux1 libopx-nas-linux-dev libopx-nas-interface1 libopx-nas-interface-dev libopx-nas-acl1 libopx-nas-acl-dev libopx-nas-l2-1 libopx-nas-l2-dev libopx-nas-l3-1 libopx-nas-l3-dev libopx-nas-qos1 libopx-nas-qos-dev libopx-nas-platform-s6000-1 libopx-sai-common-utils1 libopx-sai-common1

> **NOTE**: The `opx_build` command uses the S6000 platform library and will not effect runtime behavior (can be used on the virtual machine (VM) or any platform).

(c) Dell 2017
