## Como unir los 3 bloques(HTML-CSS-JS)? 

En el ```index.html``` tenemos que linquear el CSS para darle estilos y el JS para darle comportamiento a nuestra página web.

El CSS lo linqueamos con el tag ```link``` y escribimos la ruta dónde se encuentra en el atributo ```href```.

```
<head>
    <meta charset="UTF-8">
    <title>My web page</title>
    <link rel="stylesheet" type="text/css" href="styles.css">
</head>

```


El JS lo linqueamos con el tag ```script``` al final, justo antes de cerrar el ```</body>``` y escribimos la ruta dónde se encuentra en el atributo ```src```.

```
<body>
    ..
    ...
    // code here
    ...
    ...
    <script type="text/javascript" src="main.js"></script>
</body>
```

La estructura de tu proyecto debería quedar parecida a esto:

![sreenshot](https://i.imgur.com/31HaLn9.png)