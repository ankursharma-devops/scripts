This ansile play book adds a user to mulitiple servers providing him access to certain groups 
and forcing the new user to reset its password during the first login.

Usage:

ansible-playbook users.yml --extra-vars " target_servers=HOST_TAG user_name=NAME_OF_USER_TO_CREATE action=del_user/add_user/disable_user groups_name=GROUP_NAME/NA" -u ansible -k

Note: Omit the -k option if ssh agent is in use.
