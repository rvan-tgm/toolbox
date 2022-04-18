<h1> AUR - Arch User Repository </h1>
Robin van Dyck 18.04.2022
<h2> Installation </h2>

Package im AUR raussuchen und den  `GIT Clone URL` kopieren und das Repo lokal clonen

In den Ordner gehen und `makepkg -si` ausführen

<h2> Anpassen der PKGBUILD</h2>

Falls man wegen Dependencie Problemen die `PKGBUILD` oder `package.sh` anpassen muss einfach mit Editor wie Nano/Vim editieren.

Danach muss noch `updpkgsums` im Ordner von der Angepassten `PKGBUILD` ausgeführt werden, damit es beim überprüfen der Checksums während der Installation zu keinen Fehlern kommt
