## 0.9.1 (release date: 2013-11-12)

 * Improved init process script (`/sbin/my_init`): it now handles shutdown correctly. Previously, `docker stop` would not have any effect on `my_init`, causing the whole container to be killed with SIGKILL. The new init process script gracefully shuts down all runit services, then exits.

## 0.9.0 (release date: 2013-11-12)

 * Initial release
