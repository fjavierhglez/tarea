# Date
Año a cuatro digitos mes y dia

### Se compila desde la terminal con :
```bash
javier@Javier-pc:~$ date -u +"%Y-%m-%d"
```
### Resultado :
```bash
2019-05-03
```

# Which 
muestra la ruta absoluta del programa

### Se compila desde la terminal con :
```bash
javier@Javier-pc:~$ which firefox
```
### Resultado :
```bash
/usr/bin/firefox
```


# PS
Muestra los procesos activos en ese momento en esa sesion

### Se compila desde la terminal con :
```bash
javier@Javier-pc:~$ ps
```
### Resultado :
```bash
  PID TTY          TIME CMD
 5169 pts/0    00:00:00 bash
 5394 pts/0    00:00:00 ps
```

# History
muestra el historial de la temrinal

### Se compila desde la terminal con :
```bash
javier@Javier-pc:~$ history
```
### Resultado :
```bash
  1  ls directorio1
  2  cp directorio1/hola.txt directorio1/hola2.txt
  3  ls directorio1
  4  sudo apt install bc
  5  bc
  ...
  337  clear
  338  ps
  339  clear
  340  history
```


# Less
puede navegar en el texto que recibe como parametro

### Se compila desde la terminal con :
```bash
javier@Javier-pc:~$ less ordenadores.txt
```
### Resultado :
```bash
cpu1 5GB
cpu2 4GB
ordenadores.txt (END)
```


# Who
Muestra el usuario activo

### Se compila desde la terminal con :
```bash
javier@Javier-pc:~$ who
```
### Resultado :
```bash
javier@Javier-pc:~$ who
```


# Uptime
muestra el tiempo que lleva encendido el equipo

### Se compila desde la terminal con :
```bash
javier@Javier-pc:~$ uptime
```
### Resultado :
```bash
 11:11:49 up  1:59,  1 user,  load average: 0.22, 0.17, 0.18
```


# Telnet
Donde $IP es una ip real y $PORT es un puerto.

### Se compila desde la terminal con :
```bash
telnet 127.0.0.1 22
```
### Resultado :
```bash
Trying ::1...
Connected to localhost.
Escape character is '^]'.
```
Nos muestra si el puerto esta activo se cierra con Ctrl+]
y Ctrl+d


# SU
su hace un cambio de sesión de usuario, pero sin necesidad de cerrar la sesión del usuario actual.

### Se compila desde la terminal con :
```bash
javier@Javier-pc:~$ su
```
En este caso pedira la contraseña para hacer el cambio y listo
### Resultado :
```bash
Contraseña: 
```


# SUDO
ejecuta x comando temporalmente con privilegios de otro usuario "suele ser el superusuario"
$ sudo <comando>
### Se compila desde la terminal con :
```bash
javier@Javier-pc:~$ sudo firefox
```
En este caso pedira la contraseña para hacer ejecutar el comando
### Resultado :
```bash
javier@Javier-pc:~$ sudo firefox
[sudo] password for javier: XXX
Running Firefox as root in a regular user's session is not supported.  ($XAUTHORITY is /run/user/1000/gdm/Xauthority which is owned by javier.)

```


# NMAP
escanea ciertos puertos específicos, entre rangos IP específicos y el uso de paquetes

### Se compila desde la terminal con :
```bash
javier@Javier-pc:~$ nmap -Pn localhost
```
### Resultado :
```bash
Starting Nmap 7.40 ( https://nmap.org ) at 2019-05-03 11:23 CDT
Nmap scan report for localhost (127.0.0.1)
Host is up (0.00022s latency).
Other addresses for localhost (not scanned): ::1
All 1000 scanned ports on localhost (127.0.0.1) are closed

Nmap done: 1 IP address (1 host up) scanned in 0.15 seconds
```


# TRACEROUTE
traceroute $IP
herramienta de diagnóstico, que igual que ping, envía una serie de paquetes, con la diferencia que nos muestra la ruta que toma hasta el destino

### Se compila desde la terminal con :
```bash
javier@Javier-pc:~$ traceroute google.com
```
### Resultado :
```bash
traceroute to google.com (172.217.15.14), 30 hops max, 60 byte packets
 1  gateway (192.168.1.10)  24.094 ms  30.925 ms  32.987 ms
 2  10.151.0.2 (10.151.0.2)  40.019 ms  40.034 ms  40.026 ms
 3  * * *
 4  10.180.55.4 (10.180.55.4)  43.096 ms  43.103 ms  43.104 ms
 5  10.190.41.192 (10.190.41.192)  55.777 ms  55.773 ms  56.594 ms
 6  10.180.54.68 (10.180.54.68)  73.693 ms  28.551 ms  20.797 ms
 7  10.180.200.171 (10.180.200.171)  31.152 ms  31.028 ms  30.899 ms
 8  74.125.147.230 (74.125.147.230)  34.308 ms  34.274 ms  34.238 ms
 9  108.170.254.1 (108.170.254.1)  34.186 ms 108.170.254.17 (108.170.254.17)  33.997 ms  33.873 ms
10  209.85.243.15 (209.85.243.15)  33.916 ms  33.826 ms 209.85.244.137 (209.85.244.137)  33.784 ms
11  qro01s18-in-f14.1e100.net (172.217.15.14)  30.820 ms  35.194 ms  35.694 ms
```


# BC
bc es una potente calculadora que nos permite hacer calculos hasta donde te lo permita tu hadware

### Se compila desde la terminal con :
```bash
javier@Javier-pc:~$ bc
bc 1.06.95
Copyright 1991-1994, 1997, 1998, 2000, 2004, 2006 Free Software Foundation, Inc.
This is free software with ABSOLUTELY NO WARRANTY.
For details type `warranty'.
```
aquí ya habri la aplicacion desde la consola y solo queda ingresar las variables y las operaciones
### operaciones :
```bash
5+2
```
### Resultado :
```bash
7
```
con quit sales de la aplicacion


# PING
ping sirve para rastreo de paquetes de informacion

### Se compila desde la terminal con :
```bash
javier@Javier-pc:~$ ping localhost
```
### Resultado :
```bash
PING localhost(localhost (::1)) 56 data bytes
64 bytes from localhost (::1): icmp_seq=1 ttl=64 time=0.043 ms
64 bytes from localhost (::1): icmp_seq=2 ttl=64 time=0.057 ms
64 bytes from localhost (::1): icmp_seq=3 ttl=64 time=0.079 ms
64 bytes from localhost (::1): icmp_seq=4 ttl=64 time=0.085 ms
--- localhost ping statistics ---
14 packets transmitted, 4 received, 0% packet loss, time 13289ms
rtt min/avg/max/mdev = 0.043/0.074/0.088/0.013 ms
```


# | PIPES
uso del simbolo pipe " | "
funciona para llevar informacion de un comando a otro

En este ejemplo echo imprime la palabra helloy wc -c hace un recuento de caracteres
### Se compila desde la terminal con :
```bash
javier@Javier-pc:~$ echo hola como estas | wc -c
```
### Resultado :
```bash
16
```
# < PIPES
uso del simbolo pipe " > "
funciona para llevar informacion de un comando a otro

En este ejemplo con el comando ls manda el resultado a txt
### Se compila desde la terminal con :
```bash
# | PIPES
uso del simbolo pipe " | "
funciona para llevar informacion de un comando a otro

En este ejemplo echo imprime la palabra helloy wc -c hace un recuento de caracteres
### Se compila desde la terminal con :
```bash
javier@Javier-pc:~$ ls > archivo2.txt
```
### Resultado :
```bash
javier@Javier-pc:~$ ls
archivo2.txt
ordenadores.txt
Plantillas.pdf
```


# TOP
muesta todos los procesos y aplicaciones que se estan ejecutando
### Se compila desde la terminal con :
```bash
javier@Javier-pc:~$ top
```
### Resultado :
```bash
top - 12:06:02 up  2:53,  1 user,  load average: 0.82, 0.80, 0.69
Tasks: 228 total,   1 running, 227 sleeping,   0 stopped,   0 zombie
%Cpu(s):  3.5 us,  1.3 sy,  0.0 ni, 94.7 id,  0.3 wa,  0.0 hi,  0.1 si,  0.0 st
KiB Mem :  7835276 total,  4146388 free,  2083908 used,  1604980 buff/cache
KiB Swap:  5858300 total,  5858300 free,        0 used.  5149276 avail Mem 

  PID USER      PR  NI    VIRT    RES    SHR S  %CPU %MEM     TIME+ COMMAND     
 1051 javier    20   0  324468  53160  20560 S   5.0  0.7   7:55.81 Xorg        
 1140 javier    20   0 2351772 207048  63336 S   3.6  2.6  10:02.33 gnome-shell 
 7827 javier    20   0  756380 136636  80192 S   3.6  1.7   0:09.67 chrome      
 1552 javier    20   0 1701520 309944 121288 S   3.3  4.0  10:22.86 chrome      
 5163 javier    20   0  647212  36280  27852 S   2.3  0.5   0:15.00 gnome-term+ 
 5491 javier    20   0  831384 160952  82736 S   2.3  2.1   2:43.21 chrome      
 1167 javier     9 -11 1618596  11284   8440 S   1.3  0.1   1:10.89 pulseaudio  
 7787 javier    20   0  718240 109912  71596 S   1.3  1.4   0:06.16 chrome      
 8022 javier    20   0   45004   3836   3104 R   1.0  0.0   0:00.74 top  
```



# SLEEP
sleep $Ns #donde N es un numero
El comando sleep que fija un tiempo para llevar a cabo una acción. Es como un cronometro, cuando termina la cuenta se realiza la acción que le sigue
### Se compila desde la terminal con :
```bash
javier@Javier-pc:~$ sleep 3s; echo "Hola"
```
### Resultado :
```bash
Hola
```






