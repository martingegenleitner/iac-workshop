# IaC Workshop

Small setup to demonstrate the use of vagrant, ansible and kubernetes

## How to start

* Install [vagrant](https://developer.hashicorp.com/vagrant/install) and [virtualbox](https://www.virtualbox.org/wiki/Downloads)
* Change into this as your working directory.
* Run `vagrant up` to spin up the VM.
* Run `vagrant ssh` to access the VM.
* Check with `microk8s status`, if your kubernetes cluster is up and running.
* Use `k` as an alias for `kubectl` to access the local kubernetes cluster and play around with it.

## How to use helm and kubectl directly

Running as user `vagrant` execute `microk8s config > ~/.kube/config` to create a proper kubectl config.

## Docs

* About microk8s: <https://ubuntu.com/tutorials/install-a-local-kubernetes-with-microk8s#1-overview>
* About vagrant
  * Used box from <https://portal.cloud.hashicorp.com/vagrant/discover/gutehall/ubuntu24-04>
  * Docs for ansible_local at <https://developer.hashicorp.com/vagrant/docs/provisioning/ansible_local>
