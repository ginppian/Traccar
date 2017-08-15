Traccar
=====

## Definición

<p align="justify">
	Traccar según su <a href="https://github.com/tananaev/traccar">documentación oficial</a> <i> "is open source server for various GPS tracking devices. Project is written in Java and works on most platforms with installed Java Runtime Environment."</i> Y se distribuye bajo licencia <i>Apache 2.0</i>.
</p>

## Instalación

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
		</ul>
	</li>
</ol>

## Fuente

* <a href="https://www.traccar.org/forums/topic/how-to-install-traccar-server-on-vps/">How to install Traccar server on VPS</a>
* <a href="http://lobotuerto.com/blog/2014/08/26/como-instalar-oracle-java-en-ubuntu/">Cómo instalar Oracle Java 8 en Ubuntu 16.04</a>

