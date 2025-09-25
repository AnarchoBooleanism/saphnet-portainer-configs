## Media server
A media server designed to integrate with the Deluge Seedbox, using Jellyfin, Jackett, and Radarr.

For ideal results, make sure your virtual machine has access to a GPU with good transcoding support.

This setup is designed to work with an NFS server, with a central directory for a media server, with the following subdirectories:
- `jellyfin`: Has the subdirectories `config` and `cache`, for Jellyfin to directly interact with.
- `deluge`: Has the subdirectories `torrent_files` and `torrent_downloads`, respectively for .torrent files and completed downloads, which the Deluge Seedbox deals with.
- `movies`: A directory that contains movie files.