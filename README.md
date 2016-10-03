# Grafana Riak TS Datasource Vagrant Demo

[![License](https://img.shields.io/badge/license-apache-blue.svg?style=flat)](https://github.com/glickbot/grafana-riakts-demo/blob/master/LICENSE)

*NOT YET WORKING*

Vagrant Demo for Riak TS + Grafana + Riak Explorer

## Usage

### Requirements
- [Vagrant](https://www.vagrantup.com/)
- [Ansible 2.1+](https://www.ansible.com/)
- Riak TS Grafana Datasource

### Steps
    clone https://github.com/glickbot/grafana-riakts-demo
    cd grafana-riakts-demo
    git clone <grafana-riakts-datasource uri>
    ansible-galaxy install -r requirements.yml
    vagrant up