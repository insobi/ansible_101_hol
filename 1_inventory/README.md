# Hands-on - Inventory

#### Case 1
```
ansible -i hosts.ini all -m ping
```

#### Case 2
```
ansible -i hosts.ini all -a hostname
ansible -i hosts.ini web -a hostname
ansible -i hosts.ini web,was -a hostname
ansible -i hosts.ini "*2" -a hostname
```

#### Case 3
```
ansible -i hosts.ini all -a id
ansible -i hosts.ini all -a id -b -u root
```