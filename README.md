# DLNA nginx module

DLNA (Digital Living Network Alliance) makes it possible to share
video and audio from your computer to other media devices like TV.

## Build

Add module when configuring nginx

    ./configure --add-module=/path/to/nginx-dlna-module ...

## Directives

### dlna [NAME]

NAME is DLNA resource name. If omitted location name is used.

    location /dlna {
        dlna "My Video";
        alias /home/user/Videos;
    }
