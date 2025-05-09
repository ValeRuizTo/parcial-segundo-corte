
### API

https://segundo-parcial-ochre.vercel.app/


###  Valentina Ruiz






### Instrucciones Generales
- Una ruta de una API REST desarrollada con Express, todas deben desarrollarse dentro de la misma aplicación.
- Utiliza la versión más reciente de Express para desarrollar la API.
- Utiliza las buenas prácticas de desarrollo que has aprendido en clase.
- La evaluación se realizará en base a la funcionalidad correcta de las rutas, la claridad del código y la organización de tu aplicación.
- Es importante que esta API esté desplegada y funcionando correctamente. Si la API no está desplegada en internet, el examen no será calificado y se otorgará una calificación de 0.

### Rutas
1. **/coin/:coinName**
   - Descripción: Este endpoint debe consumir la API de CoinCap (https://docs.coincap.io/?version=latest) y recibir por parámetro el nombre de una moneda. Si el nombre de la moneda es válido, debe retornar un string con el siguiente formato: "El precio en dólares de la moneda para el día de hoy es X", donde X es el precio de la moneda en dólares según CoinCap. Si el nombre de la moneda no es válido, debe retornar un mensaje diciendo "El nombre de la moneda no fue encontrado en la base de datos".

2. **/users/:count?sort=ASC|DESC**
   - Descripción: Este endpoint debe retornar una lista de usuarios. El parámetro count indica la cantidad de usuarios a devolver y el parámetro sort indica si la lista debe estar organizada de manera ascendente (ASC) o descendente (DESC) según el apellido del usuario. Por defecto, la lista debe estar organizada de manera ascendente. La lista debe contener al menos nombre y apellido de cada usuario.

3. **/users**
   - Descripción: Este endpoint debe simular la creación de un usuario. Debe recibir los siguientes parámetros obligatorios: nombre, apellido, correo electrónico. Además, puede recibir los parámetros opcionales ciudad y país. Si no se proporcionan ciudad ni país, estos deben ser seteados por defecto a "Bogotá" y "Colombia" respectivamente. Una vez "creado" el usuario, el endpoint debe retornar un objeto JSON con la información del usuario creado.
