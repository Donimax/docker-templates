# Unraid Docker-Templates

## DockerTemplateSchema documentation

[DockerTemplateSchema](https://wiki.unraid.net/DockerTemplateSchema)

## Since 6.10.0 Stable

The Template Repositories section of the OS is now removed

### Solution

If you are one of the 0.001% of users that is still currently using it, there are 2 completely viable alternatives listed in this thread (put the xml's into either /config/plugins/dockerMan/templates-user or /config/plugins/community.applications/private/myNameHere)

- clone into repo `/boot/config/plugins/community.applications`
- rename repo to `private`

### Script to pull template updates

```bash
#!/bin/bash

#Change to private template repo
cd /boot/config/plugins/community.applications/private
#Pull private repo
git pull

# Clean exit
exit 0
```

## Docker Templates User location

```bash
/boot/config/plugins/dockerMan/templates-user
```
