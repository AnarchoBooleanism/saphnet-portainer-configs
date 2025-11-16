# saphnet-compose-configs
A set of configuration files for different Docker Compose stacks for Komodo to pull from and run

## Where to deploy each stack

### portainer-control (portainer.int-net.saphnet.xyz)
- `docker-proxy`
- `docker-volume-rclone`

### docker-nginx (nginx.int-net.saphnet.xyz)
- `docker-volume-rclone`
- ALL stacks in `nginx-stacks`. Make sure the host has access to the Tailscale network as well.

### docker-main-pve1 (docker-main.pve1.int-net.saphnet.xyz)
- `docker-proxy`
- `docker-volume-rclone`
- `netbootxyz`

### docker-main-pve3 (docker-main.pve3.int-net.saphnet.xyz)
NOTE: This host has an Intel Arc A310 for GPU acceleration.
- `docker-proxy`
- `docker-volume-rclone`
- `deluge-seedbox`
- `foldingathome` (Can be deployed anywhere, but GPU on host preferred, and ideally CUDA)
- `media-server` (Should be deployed on hosts that have a good GPU for transcoding)

### docker-main-pve4 (docker-main.pve4.int-net.saphnet.xyz)
- `docker-proxy`
- `docker-volume-rclone`

**TODO:**
- Find way of automating writing down volumes for docker-volume-rclone
