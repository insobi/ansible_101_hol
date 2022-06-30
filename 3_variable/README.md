# Variable

#### Case 1 - vars
```
ansible-playbook -i hosts.ini pb_vars.yml
```

#### Case 2 - vars_files
```
ansible-playbook -i hosts.ini pb_vars_files.yml
```

#### Case 3 - extra_vars
```
ansible-playbook -i hosts.ini  pb_extra_vars.yml --extra-vars host=web1
ansible-playbook -i hosts.ini  pb_extra_vars.yml -e host=web
ansible-playbook -i hosts.ini  pb_extra_vars.yml -e host=all
```

#### Case 4 - set_facts
```
ansible-playbook -i hosts.ini pb_set_fact.yml
```

#### Case 5 - register
```
ansible-playbook -i hosts.ini pb_register.yml
```