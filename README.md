# saphnet-portainer-configs
A set of configuration files for different Portainer stacks for Portainer to pull from and run

## Where to deploy each stack

### portainer-control (portainer.int-net.saphnet.xyz)
- `docker-proxy`

### docker-nginx (nginx.int-net.saphnet.xyz)
- ALL stacks in `nginx-stacks`. Make sure the host has access to the Tailscale network as well.

### docker-main-pve1 (docker-main.pve1.int-net.saphnet.xyz)
- `docker-proxy`
- `netbootxyz`

### docker-main-pve3 (docker-main.pve3.int-net.saphnet.xyz)
NOTE: This host has an Intel Arc A310 for GPU acceleration.
- `docker-proxy`
- `deluge-seedbox`
- `foldingathome` (Can be deployed anywhere, but GPU on host preferred, and ideally CUDA)
- `media-server` (Should be deployed on hosts that have a good GPU for transcoding)

### docker-main-pve4 (docker-main.pve4.int-net.saphnet.xyz)
- `docker-proxy`