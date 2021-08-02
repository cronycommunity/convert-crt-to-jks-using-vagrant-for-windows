# install-jenkins-using-vagrant-on-vm

## Install VM

https://www.virtualbox.org/

## Install Vagrant

https://www.vagrantup.com/docs/installation

## Open project directory and run this command

``` 1
vagrant up
```

# If you change Vagrantfile, run this command to update

```
vagrant reload --provision (not required)
```

# Go 192.168.33.10:8080 to open Jenkins

# VM Server Connection
``` 2
vagrant ssh
```


# Create jks file
You should add your crt and key file in files with 'ca' name

``` 3
sh run1.sh
```

``` 4
sh run2.sh
```

After this commands and your passwords, you can see your jks file in files folder.

Mete  | Demirtas
------------- | -------------
