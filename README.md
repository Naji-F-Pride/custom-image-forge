# custom-image-forge
Workshop for Packet custom images and custom image creation tools.

Create custom images with `image-creator`.

Prerequisits:
* Docker
* PV
* tar
* jq
* mktemp

Download and edit the packet Dockerfile to your liking.
```
wget https://raw.githubusercontent.com/packethost/packet-images/ubuntu_16_04-base/x86_64/Dockerfile
nano Dockerfile
```
Run `image-creator` and specify the ubuntu version and architecture.
```
./image-creator -v 16.04 -a x86_64
```
You can also specify the ouput directory with `-o` and turn on verbose output with `-V`.
