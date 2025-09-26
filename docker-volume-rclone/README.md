## docker-volume-rclone
A solution for regularly cloning Docker volumes to a remote NFS location.

Should be customized for each machine, with each machines' volumes all mapped to subdirectories within `/volumes`. Make sure to update these configs when changing anything related to volumes.

For setup, make sure to refer to [the documentation of the image repo](https://github.com/AnarchoBooleanism/docker-volume-rclone).