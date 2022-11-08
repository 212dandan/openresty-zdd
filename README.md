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
[root@zdd bin]# cd /usr/local/openresty/bin
[root@zdd bin]# ls
md2pod.pl  nginx-xml2pod  openresty  opm  resty  restydoc  restydoc-index
[root@zdd bin]# ./resty -V
resty 0.28
nginx version: openresty/1.19.9.1
built by gcc 8.3.0 20190222 (Loongson 8.3.0-31 vec) (GCC) 
built with OpenSSL 1.0.2k  26 Jan 2017
TLS SNI support enabled
configure arguments: --prefix=/usr/local/openresty/nginx --with-cc-opt=-O2 --add-module=../ngx_devel_kit-0.3.1 --add-module=../echo-nginx-module-0.62 --add-module=../xss-nginx-module-0.06 --add-module=../ngx_coolkit-0.2 --add-module=../set-misc-nginx-module-0.32 --add-module=../form-input-nginx-module-0.12 --add-module=../encrypted-session-nginx-module-0.08 --add-module=../srcache-nginx-module-0.32 --add-module=../ngx_lua-0.10.20 --add-module=../ngx_lua_upstream-0.07 --add-module=../headers-more-nginx-module-0.33 --add-module=../array-var-nginx-module-0.05 --add-module=../memc-nginx-module-0.19 --add-module=../redis2-nginx-module-0.15 --add-module=../redis-nginx-module-0.3.7 --add-module=../rds-json-nginx-module-0.15 --add-module=../rds-csv-nginx-module-0.09 --add-module=../ngx_stream_lua-0.0.10 --with-ld-opt=-Wl,-rpath,/usr/local/openresty/luajit/lib --with-openssl=/root/openresty-zdd/openssl-1.0.2k --with-pcre=/root/openresty-zdd/pcre-8.42 --with-zlib=/root/openresty-zdd/zlib-1.2.11 --with-http_stub_status_module --with-openssl-opt=-g --with-pcre-opt=-g --with-zlib-opt=-g --with-stream --with-stream_ssl_module --with-stream_ssl_preread_module --with-http_ssl_module
