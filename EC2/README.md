# Ansible PoC for AWS Ubuntu

After provisioning you ubuntu servers check if you are able to ping them first.

```
$ ansible -m ping -i /Users/wendy/ansible/EC2/aws_ec2.yml  all    
```