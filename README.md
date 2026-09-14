
# Holodeck 🖖

Machines Virtuelles Web pour les Ingénieurs de Starfleet — infrastructure Debian sécurisée avec Nginx, PHP 7/8, MariaDB, LDAP, FTPS et pare-feu.

# Télécharger les VM
Machine	Description:
VM Serveur	Debian sans interface graphique — DHCP/DNS, Nginx, PHP-FPM 7.4/8.3, MariaDB, LDAP, FTPS, pare-feu
VM Cliente	Debian avec interface graphique (MATE) — poste de test

⚠️ Les fichiers .ova étant trop volumineux pour GitHub, ils sont hébergés séparément.
Lien vers les VM
https://drive.google.com/drive/folders/1fsxLFf05ldNIZeNGmED-1IE7V71cZj79?usp=sharing

# Documentation
NOTICE_INSTALLATION_UTILISATION.md — installation de VMware, import des VM, premier démarrage, accès aux services
PROCEDURE_EXPORT_VM.md — procédure d'export des VM
backup_starfleet.sh — script de sauvegarde automatisé de la configuration serveur

# Infrastructure
Réseau : DHCP/DNS internes (domaine starfleet.lan)
Web : Nginx (HTTPS) + PHP-FPM 7.4 et 8.3 en cohabitation + MariaDB
Annuaire : OpenLDAP, utilisé pour l'authentification sur le site web
Fichiers : FTPS chrooté par site
Sécurité : pare-feu nftables, aucun compte sudo, administration en root par clé SSH
Bonus : VS Code Server, script de sauvegarde automatisé (cron)

# Services
Service	Adresse
Site web PHP 8	https://www8.starfleet.lan
Site web PHP 7	https://www7.starfleet.lan
phpMyAdmin	https://php.starfleet.lan
Cockpit (admin)	https://admin.starfleet.lan
VS Code Server	https://vscore.starfleet.lan
FTP (FTPS)	ftp.starfleet.lan

