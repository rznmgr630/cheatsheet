# Problems

## 1. ENOSPC: System limit for number of file watchers reached
### Temporary Solution
1. Open this file
   `sudo nano /etc/sysctl.conf`
2. Add this line at the end of the file
   `fs.inotify.max_user_watches=524288`
3. Apply the changes
   `sudo sysctl -p`
