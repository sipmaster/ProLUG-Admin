
```bash
dnf whatprovides ansible
```
```bash
Last metadata expiration check: 1:57:58 ago on Thu Aug 14 17:15:56 2025.
ansible-1:7.7.0-1.el9.noarch : Curated set of Ansible collections included in addition to ansible-core
Repo        : epel
Matched from:
Provide    : ansible = 1:7.7.0-1.el9
```
```bash
ansible --version
ansible [core 2.16.3]
  config file = None
  configured module search path = ['/root/.ansible/plugins/modules', '/usr/share/ansible/plugins/modules']
  ansible python module location = /usr/lib/python3/dist-packages/ansible
  ansible collection location = /root/.ansible/collections:/usr/share/ansible/collections
  executable location = /usr/bin/ansible
  python version = 3.12.3 (main, Jun 18 2025, 17:59:45) [GCC 13.3.0] (/usr/bin/python3)
  jinja version = 3.1.2
  libyaml = True
```
```bash
ansible-doc -l | wc -l
8354
```
```bash
ansible-inventory -i /root/hosts --graph
[WARNING]: Invalid characters were found in group names but not replaced, use -vvvv to see details
@all:
  |--@ungrouped:
  |--@prod_env:
  |  |--controlprod
  |  |--node01prod
  |--@non-prod:
  |  |--@servers:
  |  |  |--controlplane
  |  |  |--node01
  |  |--@test_env:
  |  |  |--controltest
  |  |  |--node01test
controlplane:~$ ansible-inventory -i /root/hosts --list -y
[WARNING]: Invalid characters were found in group names but not replaced, use -vvvv to see details
all:
  children:
    non-prod:
      children:
        servers:
          hosts:
            controlplane: {}
            node01: {}
        test_env:
          hosts:
            controltest:
              type: client
            node01test:
              type: server
    prod_env:
      hosts:
        controlprod:
          type: client
        node01prod:
          type: server
```
```bash
ansible servers -i /root/hosts -m shell -a 'uptime'
node01 | CHANGED | rc=0 >>
 18:16:30 up 48 min,  0 user,  load average: 0.16, 0.06, 0.01
controlplane | CHANGED | rc=0 >>
 18:16:30 up 48 min,  1 user,  load average: 1.61, 0.50, 0.25
```
```bash
ansible servers -i /root/hosts -m setup -a 'filter=ansible_distribution'
node01 | SUCCESS => {
    "ansible_facts": {
        "ansible_distribution": "Ubuntu",
        "discovered_interpreter_python": "/usr/bin/python3"
    },
    "changed": false
}
controlplane | SUCCESS => {
    "ansible_facts": {
        "ansible_distribution": "Ubuntu",
        "discovered_interpreter_python": "/usr/bin/python3"
    },
    "changed": false
}
```
```bash
> {
    "ansible_facts": {
        "ansible_date_time": {
            "date": "2025-08-15",
            "day": "15",
            "epoch": "1755281892",
            "epoch_int": "1755281892",
            "hour": "18",
            "iso8601": "2025-08-15T18:18:12Z",
            "iso8601_basic": "20250815T181812543251",
            "iso8601_basic_short": "20250815T181812",
            "iso8601_micro": "2025-08-15T18:18:12.543251Z",
            "minute": "18",
            "month": "08",
            "second": "12",
            "time": "18:18:12",
            "tz": "UTC",
            "tz_dst": "UTC",
            "tz_offset": "+0000",
            "weekday": "Friday",
            "weekday_number": "5",
            "weeknumber": "32",
            "year": "2025"
        },
        "discovered_interpreter_python": "/usr/bin/python3"
    },
    "changed": false
}
controlplane | SUCCESS => {
    "ansible_facts": {
        "ansible_date_time": {
            "date": "2025-08-15",
            "day": "15",
            "epoch": "1755281892",
            "epoch_int": "1755281892",
            "hour": "18",
            "iso8601": "2025-08-15T18:18:12Z",
            "iso8601_basic": "20250815T181812917989",
            "iso8601_basic_short": "20250815T181812",
            "iso8601_micro": "2025-08-15T18:18:12.917989Z",
            "minute": "18",
            "month": "08",
            "second": "12",
            "time": "18:18:12",
            "tz": "UTC",
            "tz_dst": "UTC",
            "tz_offset": "+0000",
            "weekday": "Friday",
            "weekday_number": "5",
            "weeknumber": "32",
            "year": "2025"
        },
        "discovered_interpreter_python": "/usr/bin/python3"
    },
    "changed": false
}
controlplane:~$ 
```