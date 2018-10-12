### playbook示例
    zabbix-agent_install_demo.yml
    - hosts: all
      vars:
        - ansible_ssh_user: user
          ansible_ssh_pass: password
          zabbix_server_ip: 192.168.1.1   #必须要传递这个参数
      roles：
        - zabbix-agent