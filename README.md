# Proyectos 
Una recopilación de proyectos de **IA** en los que he trabajado.


## [OCR en recibos](https://github.com/pilarcode/demo-receipt-ocr)

Experimento para extraer texto de las imágenes de recibos y extraer features como establecimiento, precio, descripción, fecha y total de un dataset de tickets de compra.

Clasificar las compras nos permite predecir los gastos que realizará un cliente o realizar compras de forma automática.
 - [x] Implementar un servicio web para el reconocimiento de texto en imágenes como alternativa al que ya se encuentra disponible en la plataforma de Aws que es de coste.
 - [x] Explorar los datasets de facturas o recibos disponibles en el estado del arte para utilizarlo en nuestro caso de uso.
 - [x] Tarea de extracción de datos. Dada una imagen de un recibo o ticket de compra obtener el nombre del establecimiento donde se realizo la compra, fecha de la compra y el listado de los productos (establecimiento, nombre producto, precio del producto) en formato texto.
 - [ ] Tarea de almacenamiento: Guardar la información del fichero txt en una base de datos NoSQL ( por ejemplo: Amazon DynamoDB) para categorizar las compras.


![ocr example of inference](/images/ocr-extraccion-campos.png)

## [Action Recognition en videos ](https://github.com/pilarcode/action-recognition-in-videos)

Proyecto enfocado en el reconocimiento de acciones en los videos sobre un dominio concreto, el baile. Reconocer las acciones en los videos es un problema de la taxonomia video semantic understanding.  En este proyecto, se ha realizado una investigación del estado del arte. 

Además, se ha realizado un prototipo de API de reconocimiento de acciones. Para ello, en primer lugar, se entrenan dos modelos con dos approaches diferentes detallados en el paper del proyecto utilizando el dataset de Let'sDance. En segundo lugar, se implementa una API con dos servicios uno para cada modelo. Cada servicio recibe una url y devuelve un json con la etiqueta y la confianza del modelo para cada clase posible. Por ultimo, se realizan pruebas sobre videos de Youtube con estilos de baile que los modelos han aprendido (Flamenco, Ballet, Break y Waltz).


![action recognition example of inference](/images/action_recognition.png)
