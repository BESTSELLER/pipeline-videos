# Pipeline Videos

## Setting Up Videos with Git LFS

This repository uses [Git LFS](https://git-lfs.com/) to handle large video files such as MP4s and MOVs. Follow the steps below to ensure your videos are exported correctly and available via GitHub's media CDN.

### Migrating Existing Videos to Git LFS

If you have already committed and pushed video files to GitHub, run the migration command to update your repository history and move the videos to Git LFS:

```bash
git lfs migrate import --include="*.mp4,*.mov" --everything
git push --force
```

> Warning: Rewriting repository history can have side effects on collaborators. Ensure everyone is informed and take appropriate backups before migrating.
