cd /home/cloudgenius/coreos-cluster-kvm
ansible-playbook destroy.yml
rm -rf /var/lib/libvirt/dnsmasq/virbr0.status
rm -rf /home/cloudgenius/coreos-cluster-kvm/ip.md
ansible-playbook create.yml
cat /var/lib/libvirt/dnsmasq/virbr0.status
cat /home/cloudgenius/coreos-cluster-kvm/ip.md
