FROM centos:latest

# Install lmod dependencies
RUN dnf install --enablerepo=PowerTools -y lua-filesystem lua-posix

# Install OpenHPC
RUN yum install -y http://repos.openhpc.community/OpenHPC/2/CentOS_8/x86_64/ohpc-release-2-1.el8.x86_64.rpm
RUN yum install -y openmpi4-gnu9-ohpc.x86_64 lmod-ohpc

# Install git
RUN yum install -y git

# Load OpenMPI modules
# RUN /bin/bash -c "module load gnu9 && module load openmpi4"
