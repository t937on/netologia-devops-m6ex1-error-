## Домашнее задание к занятию "13.Системы мониторинга"  
  
Ошибка. Не запускаются контейнеры sandbox_kapacitor_1 и  sandbox_chronograf_1  
  
```  
$ ./sandbox logs kapacitor  
$ ./sandbox logs chronograf  
```  
  
```  
ubunter@compute-vm-2-2-10-hdd-1737113036048:~/myGitHub/netologia-devops-m6ex1-error-/sandbox$ ./sandbox logs kapacitor  
Using latest, stable releases  
Following the logs from the kapacitor container...  
Attaching to sandbox_kapacitor_1  
kapacitor_1      |   
kapacitor_1      | '##:::'##::::'###::::'########:::::'###:::::'######::'####:'########::'#######::'########::  
kapacitor_1      |  ##::'##::::'## ##::: ##.... ##:::'## ##:::'##... ##:. ##::... ##..::'##.... ##: ##.... ##:  
kapacitor_1      |  ##:'##::::'##:. ##:: ##:::: ##::'##:. ##:: ##:::..::: ##::::: ##:::: ##:::: ##: ##:::: ##:  
kapacitor_1      |  #####::::'##:::. ##: ########::'##:::. ##: ##:::::::: ##::::: ##:::: ##:::: ##: ########::  
kapacitor_1      |  ##. ##::: #########: ##.....::: #########: ##:::::::: ##::::: ##:::: ##:::: ##: ##.. ##:::  
kapacitor_1      |  ##:. ##:: ##.... ##: ##:::::::: ##.... ##: ##::: ##:: ##::::: ##:::: ##:::: ##: ##::. ##::  
kapacitor_1      |  ##::. ##: ##:::: ##: ##:::::::: ##:::: ##:. ######::'####:::: ##::::. #######:: ##:::. ##:  
kapacitor_1      | ..::::..::..:::::..::..:::::::::..:::::..:::......:::....:::::..::::::.......:::..:::::..::  
kapacitor_1      |   
kapacitor_1      | 2025/01/17 12:21:48 Using configuration at: /etc/kapacitor/kapacitor.conf  
kapacitor_1      | ts=2025-01-17T12:21:48.094Z lvl=info msg="kapacitor starting" service=run version=1.7.6 branch=HEAD commit=3347c7d9aec8e031a3eb05f501461fb106c20529  
kapacitor_1      | ts=2025-01-17T12:21:48.094Z lvl=info msg="go version" service=run version=go1.22.7  
kapacitor_1      | ts=2025-01-17T12:21:48.114Z lvl=info msg="listing Kapacitor hostname" source=srv hostname=9619d35cf5a1  
kapacitor_1      | ts=2025-01-17T12:21:48.115Z lvl=error msg="encountered error" service=run err="create server: failed to save cluster ID: open /var/lib/kapacitor/cluster.id: permission denied"  
kapacitor_1      | run: create server: failed to save cluster ID: open /var/lib/kapacitor/cluster.id: permission denied  
sandbox_kapacitor_1 exited with code 1  
ubunter@compute-vm-2-2-10-hdd-1737113036048:~/myGitHub/netologia-devops-m6ex1-error-/sandbox$ ./sandbox logs chronograf  
Using latest, stable releases  
Following the logs from the chronograf container...  
Attaching to sandbox_chronograf_1  
chronograf_1     | time="2025-01-17T12:21:55Z" level=error msg="Unable to create bolt clientUnable to open boltdb; is there a chronograf already running?  open /var/lib/chronograf/chronograf-v1.db: permission denied"  
sandbox_chronograf_1 exited with code 1  
```  
  

