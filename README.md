# Taiga: Setup production environment

yum update -y
dnf groupinstall "Development Tools"
dnf install -y libjpeg-devel zlib-devel git gdbm-devel python3 python3-pip python3-devel libxml2-devel libxslt-devel openssl-devel libffi-devel