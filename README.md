# rpmbuild-pagerduty-nagios-pl

Create a pagerduty-nagios-pl RPM for RHEL/CentOS.

## Requirements

To download package sources and install build dependencies

    yum -y install rpmdevtools yum-utils

## Build process

To build the package follow the steps outlined below

    git clone https://github.com/linuxhq/rpmbuild-pagerduty-nagios-pl.git rpmbuild
    mkdir rpmbuild/SOURCES
    spectool -g -R rpmbuild/SPECS/pagerduty-nagios-pl.spec
    yum-builddep rpmbuild/SPECS/pagerduty-nagios-pl.spec
    rpmbuild -ba rpmbuild/SPECS/pagerduty-nagios-pl.spec

## License

BSD

## Author Information

This package was created by [Taylor Kimball](http://www.linuxhq.org).
