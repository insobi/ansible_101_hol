# Hands-on - Playbook

#### Case 1 - play hosts
```
ansible-playbook -i hosts.ini pb.yml
```

#### Case 2 - Ansible Facts
```
ansible-playbook -i hosts.ini pb_gather_facts.yml
```

#### Case 3 - become, delegate_to
```
ansible-playbook -i hosts.ini pb_become.yml
```

#### Case 4 - include_tasks
```
ansible-playbook -i hosts.ini pb_include_tasks.yml
```

#### Case 5 - run once
```
ansible-playbook -i hosts.ini pb_run_once.yml
```

#### Case 6 - tags, start-at-task
```
ansible-playbook -i hosts.ini pb_tags.yml
ansible-playbook -i hosts.ini pb_tags.yml --tags foo
ansible-playbook -i hosts.ini pb_tags.yml --tags bar
ansible-playbook -i hosts.ini pb_tags.yml --tags never
ansible-playbook -i hosts.ini pb_tags.yml --tags omg
ansible-playbook -i hosts.ini pb_tags.yml --start-at-task "foo,bar"
```