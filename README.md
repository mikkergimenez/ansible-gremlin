### Setup

Create a secrets.yml file using the following command:

ansible-vault create secrets.yml

In the following format:

---
gremlin_team_id: <team_id>
gremlin_team_secret: <team_secret>




To run the playbook using this vault:

ansible-playbook --ask-vault-pass ansible.yaml -i inventory.yml -s