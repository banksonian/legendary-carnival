# WSL and SMB Mounts
I've been using WSL to use *nix tools and teqs I like when using Windows. I did have a problem though when accessing / mounting network shares in WSL. Sometimes they'd work, sometines they'd error. Weird. But I think I've worked out the cause. Mounts will only work if you've "visited" a share before starting WSL.

WSL can be restarted with
```powershell
    Get-Service LxssManager | Restart-Service
```

