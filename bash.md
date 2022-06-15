## check dir, file exists
[ -d dir ] && echo 'dir exists'
[ ! -d dir ] && echo 'dir not exists'
[ -f dir ] && echo 'file exists'
[ ! -f dir ] && echo 'file not exists'

## if
if ...; then
    ...
fi
