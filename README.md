
# Grafana Server installation


## Role variables

| Name                        | Default Value         | Description                               |
|-----------------------------|-----------------------|-------------------------------------------|
| grafana_keystone_url        | http://localhost:5000 | Keystone URL for grafana authentiacation  |
| grafana_golang_version      | go1.7.linux-amd64     | Go version to install on a system         |
| grafana_admin_password      | GrafanaPass           | Grafana admin password                    |
| grafana_mysql_host          | localhost             | Grafana DB host                           |
| grafana_mysql_db            | grafana               | Grafana backend database                  |
| grafana_mysql_user          | grafana               | Grafana database access user              |
| grafana_mysql_password      | secrete               | Grafana database access user password     |
| grafana_data_dir            | /srv/grafana          | Datadir for a grafana                     |
| grafana_log_dir             | /var/log/grafana      | Logdir for grafana                        |
|-----------------------------|-----------------------|-------------------------------------------|

## License

MIT

## OpenStack Integration

Currently Openstack/Monasca integration is blocked by non existing keystone auth plugin.

##### Grafana PR for keystone support

https://github.com/grafana/grafana/pull/3963

##### Updated Grafana repo with grafana 2.6 version and implemented keystone auth plugin

https://github.com/twc-openstack/grafana

##### Grafana monasca datasource

https://github.com/twc-openstack/grafana-plugins
