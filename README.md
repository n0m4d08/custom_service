Centos 6
#path to copy
/etc/init.d/ntp_exporter
#start
/etc/init.d/ntp_exporter start
#stop 
/etc/init.d/ntp_exporter stop
#reload
/etc/init.d/ntp_exporter reload
#create autostart
chkconfig --add ntp_exporter
#check autostart
chkconfig --list | grep ntp

Centos 7
#path to copy
/etc/systemd/system/ntp_exporter.service 
#start
systemctl start ntp_exporter.service
#stop 
systemctl stop ntp_exporter.service
#reload
systemctl reload ntp_exporter.service
#create autostart
systemctl enable ntp_exporter.service
#check autostart
systemctl is-enabled ntp_exporter.service

