# firejail-brave-sandbox
Overview  This project documents:  Using Firejail to sandbox Brave  Running Brave with restricted network or temporary home directories  Configuring Firejail profiles for custom security  Listing and managing sandboxed processes
include /etc/firejail/globals.local
include /etc/firejail/disable-common.inc
include /etc/firejail/disable-devel.inc
include /etc/firejail/disable-program.inc
include /etc/firejail/disable-passwdmgr.inc
include /etc/firejail/whitelist-var-common.inc
include /etc/firejail/whitelist-usr-share-common.inc

noblacklist ${HOME}/.config/BraveSoftware
noblacklist ${HOME}/.cache/BraveSoftware
noblacklist ${HOME}/Downloads
private-bin brave

Preserves browser configs and downloads while sandboxing
Restricts access to sensitive system areas
Runs Brave in an isolated, secure environment

Reflection / Key Learnings
Learned how to sandbox GUI applications on Linux
Gained hands-on experience with Firejail profiles and restrictions
Improved understanding of app-level security and OS isolation
Developed skills applicable for IT security, endpoint hardening, and penetration testing
Restricts access to sensitive system areas
Runs Brave in an isolated, secure environment
