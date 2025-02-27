## Install app
use the following commands to install this app  
First get it from this repo

```
bench get-app gberp_apps https://github.com/gberp2025/gberp_apps
```
add to your site
```
bench --site gberp install-app gberp_apps
```
start the frappe app
```
bench --site gberp migrate  
bench --site gberp clear-cache
bench start
```

## Update Apps
```
bench get-app gberp_apps https://github.com/gberp2025/gberp_apps
bench build
bench --site gberp migrate  
bench --site gberp clear-cache
bench restart


## Uninstall app
```
bench --site gberp remove-from-installed-apps gberp_apps
bench remove-app gberp_apps 
```