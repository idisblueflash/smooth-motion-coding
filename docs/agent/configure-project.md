This command help to input parameters during the project creation.

```
$ bash -lc 'expect <<'"'"'EOF'"'"'
spawn npm init @motion-canvas@latest my-canvas
set timeout -1
expect "Project name"
send "my-canvas\r"
expect "Project path"
send "\r"
expect "Language"
send "\r"
expect "render your animation"
send "\r"
expect eof
EOF'
```