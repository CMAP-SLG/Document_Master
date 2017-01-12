# Document_Master
CMAP Documents for Project Management

This readme document provides an overview of the DKAN SDLC process and issues that need to
be resolved to improve it.

The current issue is that the volume sizes are to small to correctly manage the software

AS RESOURCE FILES ARE EXTENSIVE AND STATIC TO THE WEBSITE. They should not be under
revision control.

The change management procedure should be updated when LVM volume sizes are large enough to
allow the actual /var/www/html/dkan directory to be under git VC.

Currently cloning or checkout of a DKAN repo/branch should be done in

/var/www/html as sudo

Example:

cd /var/www/html

sudo git clone https://github.com/CMAP-SLG/DKAN_DEV.git

This will create /var/www/html/DKAN_DEV beside the current dkan directory.

Changes should be made to files then copied into the correct location of /var/www/html/dkan

NOTE: be sure to checkout the MYSQL_DKAN database and follow the Database Change Management Instructions.

Then, after testing, be checked into the DKAN_DEV Repo.

