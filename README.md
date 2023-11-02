# Laboratorio 11

#### Instrucciones:

Siga paso a paso los comandos en este documento y grabe un video de su servidor mientras realiza el laboratorio, suba su video a Youtube y entregue el link vía GES

### NMAP

1. Si no tiene NMAP instalado en su servidor, instálelo con el siguiente comando ```sudo apt-get install nmap```.
   
2. En su casa o trabajo, escanee cuántos hosts están actualmente conectados a la red, esto lo hace con el comando ```nmap -sP 192.168.1.0/24```. (Debe cambiar la dirección de red por su dirección actual).
   
  a. Investigue qué significan los argumentos ```-sP``` en el comando anterior.

3. Identifique el sistema operativo de otro dispositivo que esté conectado a su misma red con el comando ```nmap -O 192.168.1.12```. (Debe cambiar la dirección de red por la dirección del dispositivo a escanear).

4. Escanee los puertos TCP y UDP de un host para verificar si estos están respondiendo, esto con el comando ```nmap -PN 192.168.1.12```.
   
  a. Investigue qué output dan los argumentos ```-PN```, ```-sS``` y ```-sU``` en el comando anterior.

5. Despliegue la tabla de ruteo e interfaces de algún host conectado a su red con el comando ```nmap --iflist 192.168.1.100```.

6. En su desktop corra los protocolos con los que ha estado trabajando las últimas semanas (SMTP, HTTP, etc) mientras que en el ubuntu server hace un escaneo de puertos del host desktop y muestre en su video una captura de los puertos que utilizan estos protocolos.


NMAP también tiene la opción -v que significa Verbose, indicando que se está realizando un escaneo a más detalle y despliega al usuario una mejor representación de la información que se está obteniendo. Trate de utilizar este argumento en alguno de los ejercicios anteriores.
