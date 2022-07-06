# Distance Meter

Este repositorio es un package de ROS, por lo que se puede clonar en el src de un workspace.

El codigo se desarrollo para funcionar con codigos QR cuadrados. Para los ejemplos se uso un QR de 17 x 17 cm

Para correr los códigos con los archivos .launch que se indican a continuación, recuerde hacer ejecutables los archivos .py en la ***carpeta scripts***. Puede usar el siguiente comando:
```
chmod +x *py
```

---
Puede correr los ejemplos con:
```
roslaunch distance_meter demostration1.launch
```

![alt text](https://github.com/WilberRojas/distance_meter/blob/main/images/demo1.gif)

```
roslaunch distance_meter demostration2.launch
```

![alt text](https://github.com/WilberRojas/distance_meter/blob/main/images/demo2.gif)

```
roslaunch distance_meter demostration3.launch
```

![alt text](https://github.com/WilberRojas/distance_meter/blob/main/images/demo3.gif)

---
Si quiere probarlo con su propia cámara corra:

```
roslaunch distance_meter camera.launch
```

> No olvide cambiar el dispositivo en ***image_msg_publisher.py***, linea 10:
```{python3}
cap=cv2.VideoCapture('/dev/video4')
```
> En ***distance.py***, linea 13, configure el tamaño de su codigo QR:
```{python3}
QR_size = 17 #cm
```
