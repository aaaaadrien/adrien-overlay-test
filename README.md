# adrien-overlay

## Install

### With "simple" portage :

Make sure /etc/portage/repos.conf directory exists and dev-vcs/git installed.

*curl https://raw.githubusercontent.com/aaaaadrien/adrien-overlay-test/master/repo.conf -o /etc/portage/repos.conf/adrien-overlay-test.conf*

### With eselect repository : (Calculate Linux way)

Make sure /etc/portage/repos.conf directory exists, dev-vcs/git and app-eselect/eselect-repository installed.

*eselect repository add adrien-overlay-test git https://github.com/aaaaadrien/adrien-overlay-test.git*

### With Layman

Make sure dev-vcs/git and app-portage/layman installed on your system

*curl https://raw.githubusercontent.com/aaaaadrien/adrien-overlay-test/master/repositories.xml -o /etc/layman/overlays/adrien-overlay-test.xml*

*layman -S*

*layman -a adrien-overlay-test*

## Note for Calculate Linux

To enable updates from my overlay, set to ON the cl_update_other_set with

*cl-core-variables --set update.cl_update_other_set=on*
