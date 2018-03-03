# mage-update

Four levels of upgrades are supported:

- update_secr: security updates only
- update_safe: safe package updates
- update_deep: package updates with dependencies updates
- update_full: update as hard as you can

You can tweak the behaviour with 

- cache_valid_time
- dep_clean

## do-release-upgrade and friends

Generally, we are against performing OS release upgrades on servers; there are often little things
that get broken, or configurations gone awry). Bottom line: you don't 'upgrade' between OS releases
— you destroy and rebuild with a newer version.