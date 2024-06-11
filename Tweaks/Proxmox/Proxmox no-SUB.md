# Proxmox VE No-Subscription Repository

- Offical website link :-
```
https://pve.proxmox.com/wiki/Package_Repositories#sysadmin_no_subscription_repo
```
- to remove the PoP (You do not have a valid subscription for this server.)

```
cd /usr/share/javascript/proxmox-widget-toolkit/
```
- make a backup of proxmoxlib.js file
```
cp proxmoxlib.js proxmoxlib.js.backup
```
- edit proxmoxlib.js file, At line 566 you can see 'No valid subscription',
- edit the top of it to void
```
  if (res === null || res === undefined || !res || res
                        .data.status.toLowerCase() !== 'active') {
make this line    ##  void({        
                           title: gettext('No valid subscription'),
```
- Restart the service
```
systemctl restart pveprox.service
```
for more info
```
https://github.com/CarmineCodes/Proxmox-No-Subscription-No-Problem
```
