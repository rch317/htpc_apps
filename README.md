# htpc_apps


### Basic setup
```
git clone git@github.com:rch317/htpc_apps.git
cd htpc_apps
mkdir -p /opt/media/configure/{nginx,nzbhydra,muximux,nzbget,jackett,ombi,headphones,sonarr,radarr}
mkdir -p /opt/media/download
mkdir -p /opt/media/{movies,tv,music}
docker-compose up -d
```

You still have to configure each application manually. I'm not doing everything for you!  I would
highly suggest that you create a process to perform regular backups of the /opt/media/configure
directory. I've lost this too many times to count, and re-configuring everything from scratch really
sucks the suck.

### Wish List

  - Move the configuration stuff to a container volume; any gains there?
  - Variablize this more.  Hate repeating the same values over and over.
  - Automagical configuration...
    - I'll get it there, eventually.

