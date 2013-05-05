Install_Git_On_CentOS5.9
========================

my server on Virtual Box is run by CentOS 5.9 which can not install git just by   

`$ yum install git`  

yum returns no packages found  
the solution is here:  
`$ wget http://packages.sw.be/rpmforge-release/rpmforge-release-0.5.2-2.el5.rf.i386.rpm`

`$ rpm --import http://apt.sw.be/RPM-GPG-KEY.dag.txt`  
`$ rpm -K rpmforge-release-0.5.2-2.el5.rf.i386.rpm`  
`$ rpm -i rpmforge-release-0.5.2-2.el5.rf.i386.rpm`  

`$ yum install git-all`


reference by [here](https://gist.github.com/eddarmitage/2001099)
