# Logging

## Enable Logging
Enabling the logging is easy. Just create a folder called "logs" and you're done. 
Be careful that the folder has to be created in the current working directory. That means that you have to do e.g. 
```bash
cd /home/user/raumserver/node_modules/node_raumserver/
mkdir logs
node raumserver.js
```

It is not (!) the same as 
```bash
cd /home/user/raumserver/node_modules/node_raumserver/
mkdir logs
cd /home/user/
node raumserver/node_modules/node_raumserver/raumserver.js
```
in this case raumserver would expect the logs folder in the current working directory, which in the above example would be _/home/user/logs_

After creating the logs folder, node-raumserver has to be restarted to apply the logging. 

## Define a loglevel
The loglevel is specified in the file _config/default.json_. E.g.
```JSON
{
    "raumserver": {
        //...
        "loglevel" : 2 
    }
    //...
}
```

### 0=error
### 1=warnings
### 2=info
### 3=verbose 
### 4=debug
### 5=silly

## Log rotation
_TODO_