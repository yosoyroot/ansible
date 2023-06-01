# Ansible PoC for AWS Ubuntu

Inventory will be from the dynamic inventory provided by aws_ec2 plugin

After provisioning you ubuntu servers check if you are able to ping them first.

```
$ ansible -m ping -i EC2/aws_ec2.yml  all    
```

Output should show something like below.

```
$ ansible -m ping -i EC2/aws_ec2.yml  all                         
ec2-3-84-82-186.compute-1.amazonaws.com | SUCCESS => {
    "ansible_facts": {
        "discovered_interpreter_python": "/usr/bin/python3"
    },
    "changed": false,
    "ping": "pong"
}
ec2-50-16-113-97.compute-1.amazonaws.com | SUCCESS => {
    "ansible_facts": {
        "discovered_interpreter_python": "/usr/bin/python3"
    },
    "changed": false,
    "ping": "pong"
}
ec2-54-173-26-220.compute-1.amazonaws.com | SUCCESS => {
    "ansible_facts": {
        "discovered_interpreter_python": "/usr/bin/python3"
    },
    "changed": false,
    "ping": "pong"
}
ec2-18-212-180-4.compute-1.amazonaws.com | SUCCESS => {
    "ansible_facts": {
        "discovered_interpreter_python": "/usr/bin/python3"
    },
    "changed": false,
    "ping": "pong"
}
```