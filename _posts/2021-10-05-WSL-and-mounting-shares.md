# WSL and SMB Mounts
I've enjoyed using WSL to use tools and teqs I like whn using Windows. I did have a problem though to mounting network shares in WSL. Sometimes they'd work, sometines they'd error. Weird. But I think I've worked out the cause. Mounts will only work if you've "visited" a share before starting WSL.

WSL can be restarted with
>   Get-Service LxssManager | Restart-Service

