
v1.3

* Configure Burp UI Agent
* Configure burp restore service
* Configure Burp manual delete
* Configure Burp Autoupgrade
* Activate clients from git repository
* have tests automatic for restore, backup with test client
* modify all setting for burp_server.conf
* build burp from source and have option to choose which burp version build
* Upgrade from source
* profiles_templates from defaults, so anyone can set their own, and also with good defaults profiles: profile_lnxsrv, profile_win6x, profile_win6x_drp
* burp2_add_manual_clients to have possibility to add clients from a list, also from command line
* Automated travis import, with molecule test passed (ansible-lint, idempotence, etc) for centos/systemd, ubuntu/latest, debian/8
** Tests master branch of burp when run with debian/8 (ansible_burp_server-master2 name in molecule.yml)
* burp_server_custom_lines var (to manage your own lines in burp-server.conf)
* Good defaults profiles with option to have your own profiles only copying profiles_templates var
* Remove a client from a list burp_remove_clients
* Ability to setup new port per operation (available since burp 2.1.10)
* Use notify failure by email
