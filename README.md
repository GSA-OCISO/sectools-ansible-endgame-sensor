# ansible-endgame-agent

This role installs the endgame agent on Linux

Effectively running:
  
Copy SensorLinuxInstaller-Linux-Deployment to destination
  
then...
  
```./SensorLinuxInstaller-Linux-Deployment -k <apikey> -c SensorLinuxInstaller-Linux-Deployment.cfg```
  
## Requirements:

1. Endgame sensor installer package (endgame_installer) 
2. Endgame sensor configuration file (endgame_config)
3. API key to register with Endgame management server (endgame_apikey)

Edit the vars/main.yml to reflect values of variables:

  ```endgame_installer``` OR ```endgame_installer_s3_url```

  ```endgame_config``` OR ```endgame_config_s3_url```

  ```endgame_apikey```

Place the installer and config files in files/ directory if not using S3

