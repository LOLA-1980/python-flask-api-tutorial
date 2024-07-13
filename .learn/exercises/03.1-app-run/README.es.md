# `03.1` Running your new application

Después de crear nuestra app, debemos ejecutar e inicializar la aplicación.

Cuando la aplicación se ejecute, usará tu línea de comando, ya no podrás escribir nada en ella porque el servidor de la aplicación (como por ejemplo Flask) nunca deja de ejecutarse, espera por las "requests" o solicitudes eternamente.

## 📝 Instrucciones:

1. Añade las siguientes líneas al final de tu archivo `app.py`:

```python
# Estas dos líneas siempre deben estar al final de tu archivo app.py

if __name__ == '__main__':
  app.run(host='0.0.0.0', port=3245, debug=True)
```

> Estas dos líneas deberían estar al final de tu archivo.

Ejecuta tu nuevo servidor abriendo un **nuevo terminal aparte** y escribe el siguiente comando:

```bash
$ pipenv run python src/app.py
```

> Abre una nueva terminal para ejecutar este comando.

![Running Terminal](../../assets/running-flask-app.gif?raw=true)

La forma en que funciona este comando es utilizando nuestro comando combinado `pipenv` para iniciar nuestro entorno virtual y ejecutarlo usando Python. Nuestro archivo objetivo para iniciar nuestro servidor para futuras solicitudes es `src/app.py`.
