```bash
[root@rocky14 ~]# systemctl status firewalld

● firewalld.service - firewalld - dynamic firewall daemon

          Loaded: loaded (/usr/lib/systemd/system/firewalld.service; enabled; preset: enabled)

          Active: active (running) since Wed 2025-05-21 21:57:40 MST; 10h ago

              Docs: man:firewalld(1)

      Main PID: 815 (firewalld)

            Tasks: 2 (limit: 24465)

          Memory: 24.6M

                CPU: 469ms

          CGroup: /system.slice/firewalld.service

                          └─815 /usr/bin/python3 -s /usr/sbin/firewalld --nofork --nopid

  

May 21 21:57:40 rocky14 systemd[1]: Starting firewalld - dynamic firewall daemon...
May 21 21:57:40 rocky14 systemd[1]: Started firewalld - dynamic firewall daemon.

[root@rocky14 ~]# firewall-cmd --get-zones
block dmz drop external home internal nm-shared public trusted work

[root@rocky14 ~]# firewall-cmd --list-all --zone=public
public (active)
    target: default
    icmp-block-inversion: no
    interfaces: eth0
    sources:
    services: cockpit dhcpv6-client ssh
    ports: 9100/tcp
    protocols:
    forward: yes
    masquerade: no
    forward-ports:
    source-ports:
    icmp-blocks:
    rich rules:

[root@rocky14 ~]# firewall-cmd --get-default
public

[root@rocky14 ~]# firewall-cmd --get-active-zones
public
    interfaces: eth0

[root@rocky14 ~]# firewall-cmd --list-all --zone=trusted
trusted
    target: ACCEPT
    icmp-block-inversion: no
    interfaces:
    sources:
    services:
    ports:
    protocols:
    forward: yes
    masquerade: no
    forward-ports:
    source-ports:
    icmp-blocks:
    rich rules:

[root@rocky14 ~]# ifconfig -a | grep -i flags

eth0: flags=4163<UP,BROADCAST,RUNNING,MULTICAST>    mtu 1500

lo: flags=73<UP,LOOPBACK,RUNNING>    mtu 65536

[root@rocky14 ~]# firewall-cmd --set-default-zone=work

success

[root@rocky14 ~]# firewall-cmd --get-active-zones

work

    interfaces: eth0

[root@rocky14 ~]# firewall-cmd --set-default-zone=dmz

success

[root@rocky14 ~]# firewall-cmd --get-active-zones

dmz

    interfaces: eth0

[root@rocky14 ~]# firewall-cmd --set-default-zone=public

success

[root@rocky14 ~]# firewall-cmd --get-active-zones

public

    interfaces: eth0

[root@rocky14 ~]# firewall-cmd --change-interface=virbr0 --zone dmz

success

[root@rocky14 ~]# firewall-cmd --add-source 192.168.11.0/24 --zone=public

success

[root@rocky14 ~]# firewall-cmd --get-active-zones

dmz

    interfaces: virbr0

public

    interfaces: eth0

    sources: 192.168.11.0/24

[root@rocky14 ~]# firewall-cmd --get-services

RH-Satellite-6 RH-Satellite-6-capsule afp amanda-client amanda-k5-client amqp amqps apcupsd audit ausweisapp2 bacula bacula-client bareos-director bareos-filedaemon bareos-storage bb bgp bitcoin bitcoin-rpc bitcoin-testnet bitcoin-testnet-rpc bittorrent-lsd ceph ceph-exporter ceph-mon cfengine checkmk-agent cockpit collectd condor-collector cratedb ctdb dds dds-multicast dds-unicast dhcp dhcpv6 dhcpv6-client distcc dns dns-over-tls docker-registry docker-swarm dropbox-lansync elasticsearch etcd-client etcd-server finger foreman foreman-proxy freeipa-4 freeipa-ldap freeipa-ldaps freeipa-replication freeipa-trust ftp galera ganglia-client ganglia-master git gpsd grafana gre high-availability http http3 https ident imap imaps ipfs ipp ipp-client ipsec irc ircs iscsi-target isns jenkins kadmin kdeconnect kerberos kibana klogin kpasswd kprop kshell kube-api kube-apiserver kube-control-plane kube-control-plane-secure kube-controller-manager kube-controller-manager-secure kube-nodeport-services kube-scheduler kube-scheduler-secure kube-worker kubelet kubelet-readonly kubelet-worker ldap ldaps libvirt libvirt-tls lightning-network llmnr llmnr-client llmnr-tcp llmnr-udp managesieve matrix mdns memcache minidlna mongodb mosh mountd mqtt mqtt-tls ms-wbt mssql murmur mysql nbd nebula netbios-ns netdata-dashboard nfs nfs3 nmea-0183 nrpe ntp nut opentelemetry openvpn ovirt-imageio ovirt-storageconsole ovirt-vmconsole plex pmcd pmproxy pmwebapi pmwebapis pop3 pop3s postgresql privoxy prometheus prometheus-node-exporter proxy-dhcp ps2link ps3netsrv ptp pulseaudio puppetmaster quassel radius rdp redis redis-sentinel rootd rpc-bind rquotad rsh rsyncd rtsp salt-master samba samba-client samba-dc sane sip sips slp smtp smtp-submission smtps snmp snmptls snmptls-trap snmptrap spideroak-lansync spotify-sync squid ssdp ssh steam-streaming svdrp svn syncthing syncthing-gui syncthing-relay synergy syslog syslog-tls telnet tentacle tftp tile38 tinc tor-socks transmission-client upnp-client vdsm vnc-server warpinator wbem-http wbem-https wireguard ws-discovery ws-discovery-client ws-discovery-tcp ws-discovery-udp wsman wsmans xdmcp xmpp-bosh xmpp-client xmpp-local xmpp-server zabbix-agent zabbix-server zerotier

[root@rocky14 ~]# ls /usr/lib/firewalld/services/

RH-Satellite-6-capsule.xml    dds-multicast.xml                http.xml                                                        kube-worker.xml                nfs3.xml                                            rootd.xml                            synergy.xml

RH-Satellite-6.xml                    dds-unicast.xml                    http3.xml                                                      kubelet-readonly.xml      nmea-0183.xml                                  rpc-bind.xml                      syslog-tls.xml

afp.xml                                          dds.xml                                    https.xml                                                      kubelet-worker.xml          nrpe.xml                                            rquotad.xml                        syslog.xml

amanda-client.xml                      dhcp.xml                                  ident.xml                                                      kubelet.xml                        ntp.xml                                              rsh.xml                                telnet.xml

amanda-k5-client.xml                dhcpv6-client.xml                imap.xml                                                        ldap.xml                              nut.xml                                              rsyncd.xml                          tentacle.xml

amqp.xml                                        dhcpv6.xml                              imaps.xml                                                      ldaps.xml                            opentelemetry.xml                          rtsp.xml                              tftp.xml

amqps.xml                                      distcc.xml                              ipfs.xml                                                        libvirt-tls.xml                openvpn.xml                                      salt-master.xml                tile38.xml

apcupsd.xml                                  dns-over-tls.xml                  ipp-client.xml                                            libvirt.xml                        ovirt-imageio.xml                          samba-client.xml              tinc.xml

audit.xml                                      dns.xml                                    ipp.xml                                                          lightning-network.xml    ovirt-storageconsole.xml            samba-dc.xml                      tor-socks.xml

ausweisapp2.xml                          docker-registry.xml            ipsec.xml                                                      llmnr-client.xml              ovirt-vmconsole.xml                      samba.xml                            transmission-client.xml

bacula-client.xml                      docker-swarm.xml                  irc.xml                                                          llmnr-tcp.xml                    plex.xml                                            sane.xml                              upnp-client.xml

bacula.xml                                    dropbox-lansync.xml            ircs.xml                                                        llmnr-udp.xml                    pmcd.xml                                            sip.xml                                vdsm.xml

bareos-director.xml                  elasticsearch.xml                iscsi-target.xml                                        llmnr.xml                            pmproxy.xml                                      sips.xml                              vnc-server.xml

bareos-filedaemon.xml              etcd-client.xml                    isns.xml                                                        managesieve.xml                pmwebapi.xml                                    slp.xml                                warpinator.xml

bareos-storage.xml                    etcd-server.xml                    jenkins.xml                                                  matrix.xml                          pmwebapis.xml                                  smtp-submission.xml        wbem-http.xml

bb.xml                                            finger.xml                              kadmin.xml                                                    mdns.xml                              pop3.xml                                            smtp.xml                              wbem-https.xml

bgp.xml                                          foreman-proxy.xml                kdeconnect.xml                                            memcache.xml                      pop3s.xml                                          smtps.xml                            wireguard.xml

bitcoin-rpc.xml                          foreman.xml                            kerberos.xml                                                minidlna.xml                      postgresql.xml                                snmp.xml                              ws-discovery-client.xml

bitcoin-testnet-rpc.xml          freeipa-4.xml                        kibana.xml                                                    mongodb.xml                        privoxy.xml                                      snmptls-trap.xml              ws-discovery-tcp.xml

bitcoin-testnet.xml                  freeipa-ldap.xml                  klogin.xml                                                    mosh.xml                              prometheus-node-exporter.xml    snmptls.xml                        ws-discovery-udp.xml

bitcoin.xml                                  freeipa-ldaps.xml                kpasswd.xml                                                  mountd.xml                          prometheus.xml                                snmptrap.xml                      ws-discovery.xml

bittorrent-lsd.xml                    freeipa-replication.xml    kprop.xml                                                      mqtt-tls.xml                      proxy-dhcp.xml                                spideroak-lansync.xml    wsman.xml

ceph-exporter.xml                      freeipa-trust.xml                kshell.xml                                                    mqtt.xml                              ps2link.xml                                      spotify-sync.xml              wsmans.xml

ceph-mon.xml                                ftp.xml                                    kube-api.xml                                                ms-wbt.xml                          ps3netsrv.xml                                  squid.xml                            xdmcp.xml

ceph.xml                                        galera.xml                              kube-apiserver.xml                                    mssql.xml                            ptp.xml                                              ssdp.xml                              xmpp-bosh.xml

cfengine.xml                                ganglia-client.xml              kube-control-plane-secure.xml              murmur.xml                          pulseaudio.xml                                ssh.xml                                xmpp-client.xml

checkmk-agent.xml                      ganglia-master.xml              kube-control-plane.xml                            mysql.xml                            puppetmaster.xml                            steam-streaming.xml        xmpp-local.xml

cockpit.xml                                  git.xml                                    kube-controller-manager-secure.xml    nbd.xml                                quassel.xml                                      svdrp.xml                            xmpp-server.xml

collectd.xml                                gpsd.xml                                  kube-controller-manager.xml                  nebula.xml                          radius.xml                                        svn.xml                                zabbix-agent.xml

condor-collector.xml                grafana.xml                            kube-nodeport-services.xml                    netbios-ns.xml                  rdp.xml                                              syncthing-gui.xml            zabbix-server.xml

cratedb.xml                                  gre.xml                                    kube-scheduler-secure.xml                      netdata-dashboard.xml    redis-sentinel.xml                        syncthing-relay.xml        zerotier.xml

ctdb.xml                                        high-availability.xml        kube-scheduler.xml                                    nfs.xml                                redis.xml                                          syncthing.xml

[root@rocky14 ~]# cat /usr/lib/firewalld/services/http.xml

<?xml version="1.0" encoding="utf-8"?>

<service>

    <short>WWW (HTTP)</short>

    <description>HTTP is the protocol used to serve Web pages. If you plan to make your Web server publicly available, enable this option. This option is not required for viewing pages locally or developing Web pages.</description>

    <port protocol="tcp" port="80"/>

</service>

[root@rocky14 ~]# firewall-cmd --set-default-zone=public

Warning: ZONE_ALREADY_SET: public

success

[root@rocky14 ~]# firewall-cmd --list-services

cockpit dhcpv6-client ssh

[root@rocky14 ~]# firewall-cmd --permanent --add-service ftp

success

[root@rocky14 ~]# firewall-cmd --reload

success

[root@rocky14 ~]# firewall-cmd --get-default-zone

public

[root@rocky14 ~]# firewall-cmd --list-services

cockpit dhcpv6-client ftp ssh

[root@rocky14 ~]# firewall-cmd --permanent --add-port=1147/tcp

success

[root@rocky14 ~]# firewall-cmd --reload

success

[root@rocky14 ~]# firewall-cmd --list-ports

1147/tcp 9100/tcp

[root@rocky14 ~]# firewall-cmd --permanent --remove-service=ftp

success

[root@rocky14 ~]# firewall-cmd --permanent --remove-port=1147/tcp

success

[root@rocky14 ~]# firewall-cmd --remove-service=ftp

success

[root@rocky14 ~]# firewall-cmd --remove-port=1147/tcp

success

[root@rocky14 ~]# firewall-cmd --list-services

cockpit dhcpv6-client ssh

[root@rocky14 ~]# firewall-cmd --list-ports

9100/tcp

[root@rocky14 ~]#
```