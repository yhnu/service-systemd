# quick-systemd

quick add systemd config file

## Installing

````bash
npm i -g quick-systemd
````

### Quick start

- Install service

  + pass settings in command line (see full [documentation](./doc/README.md) for all options)
  ````bash
  sudo quick-systemd --add --service my-service --cwd /path/to/service --app main.js
  ````

  + pass all settings in JSON file
  ````bash
  sudo quick-systemd --add --settings service.json
  ````

- Run the service

````bash
sudo service my-service start
sudo service my-service stop
sudo service my-service restart
````

- Uninstall service

````bash
sudo quick-systemd --remove --service my-service
````