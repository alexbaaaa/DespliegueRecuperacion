# DespliegueRecuperacion
Repositorio para realizar las prácticas de Despliegue

## Practica DNS


1. Modificamos el archivo named y named.conf.options para configurar el servicio bind9. Definiendo la escucha en IP4, la validación DNSSEC, las consultas reculsivas solo para los autorizados y el reenvío de consultas externas. 

Ambos servidores tendrian los mismos archivos cambiando la sentencia listen-on con la ip correcta en el caso del named.conf.options ambos lo copiamos en su lugar y añadimos la sentencias al provision de cada servidor 


![named](new_dns/img/named.png)
![options](new_dns/img/options.png)


2. A continuaccion definimos las zonas directas y inversas en el named.conf.local tanto de *tierra* como de *venus*

**Tierra**:

![localT](new_dns/img/localT.png)


**Venus**:

![localV](new_dns/img/localV.png)

3. Creamos los arvhivos de zona tanto directa (db.sistema.test) como inversa (db.198.168.57). Con todos los tipos de registros especificados en la practica.


![directa](new_dns/img/directa.png)
![inversa](new_dns/img/inversa.png)

## Practica Nginx

### Instalacion y configuracion de servidor web Nginex

1. Preparamos el archivo Vagranfile base con nginx y vemos que el servicio funciona correctamente


|[servidorBase](nginx/img/servidor_base.png)
*vagranFile*

|[ngixBase](nginx/img/nginxBase.png)
*nginx funcional*





