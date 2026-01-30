# ansible
My Ansible Homelab


### Collections & requirements:
<pre><code>
ansible-galaxy collection install -r requirements.yml -p ./collections
ansible-galaxy collection list
</code></pre>

### Init-Installation:
<pre><code>
First run:
ansible-playbook -u <ssh-user> -k -K -b  playbooks/bootstrap/init.yml

Second run:
ansible-playbook playbooks/bootstrap/init.yml
</code></pre>


ansible all -m gather_facts










