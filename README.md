Traccar
=====

## Definición

<p align="justify">
	Traccar según su <a href="https://github.com/tananaev/traccar">documentación oficial</a> <i> "is open source server for various GPS tracking devices. Project is written in Java and works on most platforms with installed Java Runtime Environment."</i> Y se distribuye bajo licencia <i>Apache 2.0</i>.
</p>

## Desarrollo

### Montar el servidor

<ol>
	<li>
		<p align="justify">
			Primer paso es crear un VPS (Servidor Virtual Privado) en nuestro caso usaremos <a href="https://www.digitalocean.com/">Digital Ocean</a>.
		</p>
		<p align="justify">
			Respecto a nuestrasa caracteristicas <i>técnicas</i> que usaremos son:
		</p>
		<ul>
			<li>Ubuntu 16.03 x64 (64 bits)</li>
			<li>512MB RAM</li>
			<li>20 GB SSD disk</li>
		</ul>
		<p>
			Lo básico que nos ofrece <i>Digital Ocean</i>, para una configuración más detallada asociando las llaves <i>SSH</i> se puede consultar el siguiente <a href="https://github.com/ginppian/DigitalOcean-New_Drop_UpWith_Filezilla">tutorial</a>.
		</p>
	</li>
	<li>	
		<p align="justify">
			El siguiente paso será instalar Java
		</p>
		<ul>	
			<li>	
				$ sudo add-apt-repository ppa:webupd8team/java
			</li>
			<li>	
				$ sudo apt-get update
			</li>
			<li>	
				$ sudo apt-get install oracle-java8-installer
			</li>
			<li>	
				$ sudo apt-get install oracle-java8-set-default
			</li>
			</ul>
			<p align="justify">	
					En mi caso instalé Java 8 y funcionó bien pero se pueden instalar versiones más nuevas.
			</p>
	</li>
	<li>	
		<p align="justify">
			Instalamos <i>Traccar</i>
		</p>
		<ul>	
				<li>
				$ cd /opt	
				</li>
				<li>
				$ wget https://github.com/tananaev/traccar/releases/download/v3.5/traccar-linux-64-3.5.zip
				</li>
				<li>	
				$ unzip traccar-linux-64-3.5.zip
				</li>
				<li>
				$ chmod +x traccar.run
				</li>
				<li>
				$ sudo ./traccar.run
				</li>
				<li>	
				$ sudo /opt/traccar/bin/traccar start
				</li>
		</ul>
		<p align="justify">
				Accedemos a Traccar a través de: http://youripaddress:8082
		</p>
		<p align="justify">
				En este caso instalé la versión 3.5 de Traccar pero hay más recientes, se pueden consultar 	<a href="https://github.com/tananaev/traccar/releases">aqui</a>.
		</p>
	</li>
</ol>

### Instalar la aplicación

<p align="justify">
	Traccar nos ofrece un hambiente completo incluyendo la aplicación podemos descargarla desde la <i>Play Store</i> o podemos descargar el código fuente desde <a href="https://github.com/tananaev/traccar-client-android">aquí</a> que se distribuye bajo la licencia <a href="http://www.apache.org/licenses/LICENSE-2.0">Apache 2.0</a>.
</p>
<p align="justify">
	En nuestro caso lo descargamos y generamos el APK y la instalamos.
</p>

<p align="justify">
	Se ve algo así:	
</p>
<p align="center">
	<img src="https://github.com/ginppian/Traccar/blob/master/imgs/img3.png" width="270" height="480">
</p>

<p align="justify">
	Tenemos que asignar nuestra IP o la dirección donde tenemos alojado Traccar con su respectivo puerto.	
</p>
<p align="center">
	<img src="https://github.com/ginppian/Traccar/blob/master/imgs/img4.png" width="270" height="480">
</p>

<p align="justify">
	Podemos configurar el tiempo en que se estará enviando la ubicación.
</p>
<p align="center">
	<img src="https://github.com/ginppian/Traccar/blob/master/imgs/img2.png" width="270" height="480">
</p>

<p align="justify">
	Ahora ya podremos monitorear nuestros dispositivos.
</p>
<p align="center">
	<img src="https://github.com/ginppian/Traccar/blob/master/imgs/img1.png" width="680" height="325">
</p>

## Fuente

* <a href="https://www.traccar.org/forums/topic/how-to-install-traccar-server-on-vps/">How to install Traccar server on VPS</a>
* <a href="http://lobotuerto.com/blog/2014/08/26/como-instalar-oracle-java-en-ubuntu/">Cómo instalar Oracle Java 8 en Ubuntu 16.04</a>
* <a href="https://www.traccar.org/mysql/">MySQL Database</a>

