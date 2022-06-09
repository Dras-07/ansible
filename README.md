# ansible


<h3> Commands: </h3>

<p>ansible-playbook -i inventory/prod.yml site.yml --tags "jenkins" </p>
<p>ansible-playbook -i inventory/prod.yml site.yml --tags "install"  </p>
<p> ansible-playbook -i inventory/prod.yml site.yml --tags "items"  </p>


<h3> Configuration </h3>
<ul>
  <h2> Group_vars </h2>
  <li> Ansible will look for group_vars directory </li>
  <li> Inside the group_vars directory ,  variable files will have the same name as the group name 
    <p> For Eg: admin,all </p>
  </li>
  <li> The variables in "admin" file can be used by all the machine/servers that are inside the group named "admin" in site.yml OR hostfile </li>
  <hr>
  <h2> Inventory </h2>
  <li> We can the path to inventory file OR we can run the inventory along with the ansible-playbook </li>
  <hr>
  <h2> Roles </h2>
  <li> Ansible will look for roles in "roles/role_name/tasks/main.yml" directory. </li>
  <li> We run a particular role with the help of tags. These tags will have the same name as the role_name </li>
  <hr>
  <h2> Hostfile </h2>
  <li> Hostfile path is /etc/ansible/hosts </li>
  <li> You can add the hosts here  </li>
  <hr>
  <h2> Ansible.cfg </h2>
  <li> Path is /etc/ansible/ansible.cfg </li>
  <li> Configure the paths to host file and inventory_file </li>
  <hr>
  <h2> Ansible Variable Precedence </h2>
  <li>
    <a href='https://docs.ansible.com/ansible/latest/user_guide/playbooks_variables.html#variable-precedence-where-should-i-put-a-variable'> Ansible variable_precedence 
    </a>
  </li>
    
</ul>



