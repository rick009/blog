# curl访问https错误

## cURL error 60: SSL certificate problem: unable to get local issuer certificate

将[https://curl.haxx.se/ca/cacert.pem](https://curl.haxx.se/ca/cacert.pem)保存到本地文件中（cacert.pem），然后在php.ini 中配置curl的选项

`curl.cainfo = "path_to_cert\cacert.pem"`

重启即可