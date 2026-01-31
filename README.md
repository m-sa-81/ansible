# ansible
My Ansible Homelab


### Collections & requirements:
<pre><code>
ansible-galaxy collection install -r requirements.yml -p ./collections
ansible-galaxy collection list

#Collaction upgrade:
ansible-galaxy collection install -r requirements.yml -p ./collections --upgrade
</code></pre>

### NEue Rollen anlegen:
<pre><code>
ansible-galaxy init roles/nginx
ansible-galaxy init roles/docker
</code></pre>



### Init-Installation:
<pre><code>
First run:
ansible-playbook -u <ssh-user> -k -K -b  playbooks/bootstrap/init.yml

Second run:
ansible-playbook playbooks/bootstrap/init.yml
</code></pre>


ansible all -m gather_facts




### Shutdown all:
<pre><code>
ansible-playbook playbooks/operations/shutdown_all.yml
</code></pre>






