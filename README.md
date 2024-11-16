# Robot Serial 4R Simulation

Este repositorio contiene la simulación de un robot serial 4R en ROS2 Humble. El proyecto incluye:
- Modelo URDF del robot.
- Cálculo de la cinemática directa (postura y velocidades) e inversa.
- Simulación en Gazebo con control de trayectoria en las juntas.
- Reporte en Jupyter Notebook con videos y resultados de las simulaciones.

---

## Requisitos previos

Antes de usar este proyecto, asegúrate de tener instalado lo siguiente:
- [ROS2 Humble](https://docs.ros.org/en/humble/index.html)
- [Gazebo 11](http://gazebosim.org/)
- [Python 3.8](https://www.python.org/)
- [Colcon](https://colcon.readthedocs.io/en/released/)

---

## Instalación

Sigue estos pasos para configurar el proyecto:

1. Clonar el repositorio:
   ```bash
   git clone https://github.com/tu_usuario/robot-4r-simulation.git
   cd robot-4r-simulation
Construir el proyecto:

bash
Copiar código
source /opt/ros/humble/setup.bash
colcon build
Sourcing del espacio de trabajo:

bash
Copiar código
source install/setup.bash
Uso
Lanzar la simulación en Gazebo
Para iniciar el robot en Gazebo con control de trayectoria:

bash
Copiar código
ros2 launch examen_description bringup.launch.py
Para ejecutar la cinemática inversa desde un script (ejemplo):

bash
Copiar código
ros2 run examen_description inverse_kinematics.py
Reporte
El reporte del proyecto está disponible en formato Jupyter Notebook en la carpeta report/. Puedes ejecutarlo usando:

bash
Copiar código
jupyter notebook report/Robot_4R_Simulation.ipynb
Estructura del proyecto
El repositorio está organizado de la siguiente manera:

plaintext
Copiar código
robot-4r-simulation/
├── examen_description/         # Modelo URDF y configuraciones
├── launch/                     # Archivos de lanzamiento para ROS2
├── scripts/                    # Scripts de cinemática directa e inversa
├── report/                     # Reporte en formato Jupyter Notebook
└── README.md                   # Este archivo
Contribuciones
¡Las contribuciones son bienvenidas! Sigue estos pasos para colaborar:

Realiza un fork de este repositorio.
Crea una rama para tu función o corrección:
bash
Copiar código
git checkout -b mi-nueva-funcion
Realiza tus cambios y haz un commit:
bash
Copiar código
git commit -m "Agrega mi nueva función"
Sube tus cambios al repositorio remoto:
bash
Copiar código
git push origin mi-nueva-funcion
Abre un Pull Request en GitHub.
Autores y Créditos
Este proyecto fue desarrollado por:

-Castillo Ramos Marcos Daniel
-Mendoza Suarez Carlos Manuel
-Lazos Rodarte Ilse
-Orozco Hernandez Fernanda
-Pizano Bravo Alexis
-Salazar Barrera Diego

Licencia
Este proyecto está licenciado bajo la MIT License. Consulta el archivo LICENSE para más detalles.

Referencias
Documentación oficial de ROS2: https://docs.ros.org/
Documentación de Gazebo: http://gazebosim.org/
