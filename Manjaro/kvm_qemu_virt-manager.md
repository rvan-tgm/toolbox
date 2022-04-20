<h1> KVM & QEMU + Virt-Manager GUI</h1>
Robin 18.04.2022
<h3> WHY? </h3>
KVM / QEMU ist Virtualisierung auf Hardware Ebene, sprich VM bekommt direkten zugriff auf Hardware => Performance als wäre es main boot ;) 
Besonders nützlich wenn man Windows braucht für Games/Adobe/... und die Leistung aber auch braucht, extra Performance boost wenn man 2 GPU's hat da GPU Passtrough möglich ist

<h2> Installation </h2>

Die benötigten Packete installieren <br />
`sudo pacman -S virt-manager qemu vde2 iptables-nft dnsmasq bridge-utils openbsd-netcat edk2-ovmf swtpm`

Service starten und enablen (damit er beim hochfahren automatisch gestartet wird)

```
sudo systemctl start libvirtd.service
sudo systemctl enable libvirtd.service
```

Benutzer zu 'libvirtd' Gruppe hinzufügen, damit kein Sudo gebraucht wird

`sudo usermod -a -G libvirt $USER`

