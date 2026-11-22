# Module 5: Backups & Restores

Backups are critical for disaster recovery. I use `tar` for archiving, `rsync` for synchronizing, and `cron` for automation.

## 1. Archiving with `tar`
- **Create a backup:** `tar -czvf backup.tar.gz /path/to/folder`
  - `-c` (Create), `-z` (Gzip compression), `-v` (Verbose), `-f` (File)
- **Restore a backup:** `tar -xzvf backup.tar.gz`
  - `-x` (eXtract)

## 2. Syncing with `rsync`
- `rsync -av /source/directory/ /destination/directory/`
  - `-a` (Archive mode: preserves permissions/timestamps)
  - `-v` (Verbose)

## 3. Automating Backups (Cron)
- `cron` is the Linux task scheduler used to automate repetitive jobs.
- Edit jobs with: `crontab -e`
- List jobs with: `crontab -l`
- **Cron Syntax:** `* * * * * command`
  - Minute (0-59), Hour (0-23), Day of Month (1-31), Month (1-12), Day of Week (0-7)
- **Example:** `0 2 * * * tar -czf /backup/data.tar.gz /var/www/html`
  - (Runs every day at 2:00 AM)
