

<h1>Sistema de encuestas</h1>
<h1>System Polls</h1>
<p>Construir un sistema de encuesta en el cual se pueda escoger una 
pregunta y se pueda votar </br>por las opciones que tiene disponible 
para finalmente ver la cantidad de votos que tiene cada opción de la pregunta seleccionada.</p>
</br> 

<h2>Imagen Home/inicio</h2>

![Inicio](https://user-images.githubusercontent.com/97111500/166692588-467eb2ab-f87c-4303-8e38-f7977c695d96.png)

<h2>Imagen Question</h2>

![Preguntas](https://user-images.githubusercontent.com/97111500/166692606-24606c4c-c70e-41c7-be5f-2de5e4d00d3b.png)

<h2>Imagen Result</h2>

![Resultados](https://user-images.githubusercontent.com/97111500/166692787-201d01c4-71fd-4652-8eef-d264021a6352.png)

<h2>Db Questions</h2>

![Screenshot_3](https://user-images.githubusercontent.com/97111500/166692644-7b21b15c-a1cf-4e10-adc1-bc2e66db55c5.png)

<h2>Db Choices</h2>

![Screenshot_5](https://user-images.githubusercontent.com/97111500/166692657-41ed2819-1862-4a53-a889-d4fef7ca805a.png)

</br> 
<h2>Desarrollo</h2>
<p>Para el desarrollo se emplearon:</p> 
</br> 
<li>Python 3.10</li>
<li>Django 4.0.4</li>
<li>Mysql en Alwaysdata</li>
</br> 
<p>Como se indica, los datos se manejan en Mysql en reemplazo de sqlite por lo que se requiere</br> 
actualizar modificar Settings.py: de la siguiente forma</p> </br> 

<p>
DATABASES = {</br> 
    'default': {</br> 
        'ENGINE': 'django.db.backends.mysql',</br> 
        #'NAME': BASE_DIR / 'db.sqlite3',</br> 
        'NAME' : config('NAME'), </br> 
        'USER' : config('USER'),</br> 
        'PASSWORD' : config('PASSWORD'),</br> 
        'HOST': config('HOST'),</br> 
        'PORT'  :   '3306'</br> 
    }
}</p>
<p>Y en el archvo .env:</p> </br> 
<p color:red>
NAME = 'tu dbname'</br> 
USER = 'tu dbuser'</br> 
PASSWORD = 'tu db clave*'</br> 
HOST = 'tu host en alwaysdata.alwaysdata.net'</br> 
SECRET_KEY = 'django-insecure-)g-e-n-e-r-a-d-o-portuproyecto(vl_jx097(%uwj+#x-78t1c4'</br> 
</p>

<h2>Para inciar proyecto de manera local puedes seguir estos pasos:</h2>
<li>crear archivo proyecto</li>
<li>Desde esa carpeta abrir cmd</li> 
<li>E:\documentos\excel\Escritorio\tuproyecto>python -m venv tuvirtual</li>
<li>E:\Documentos\excel\Escritorio\tuproyecto>tuvirtual\Scripts\activate.bat</li>
<li>(tuvirtual) E:\Documentos\excel\Escritorio\tuproyecto></li>
<li>pip install django</li>
<li>(tuvirtual) E:\Documentos\excel\Escritorio\tuproyecto>django-admin startproject tu-app.</li>
<li>(tuvirtual) E:\Documentos\excel\Escritorio\tuproyecto>code .</li>
<li>(tuvirtual) E:\Documentos\excel\Escritorio\tuproyecto>code .</li>
<li>En Vscode abrir terminal y ubicarse en comand promp</li>
<li>cd nombre del proyecto</li>
<li>python manage.py runserver</li>


