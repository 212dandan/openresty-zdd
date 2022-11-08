# openresty-zdd
version: openresty-1.19.9.1 <br>
from: https://openresty.org/en/download.html <br>
info: the version of openresty-zdd that has been adapted to the loongarch architecture <br>
<br>
## build method
./configure --with-openssl=./openssl-1.0.2k --with-pcre=./pcre-8.42  --with-zlib=./zlib-1.2.11 --with-http_stub_status_module <br>
make or gmake <br>
make install or gmake install <br>
<br>
## test
[root@zdd sbin]# pwd <br>
/usr/local/openresty/nginx/sbin <br>
[root@zdd sbin]# ./nginx -version
nginx version: openresty/1.19.9.1
