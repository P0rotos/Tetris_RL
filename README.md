Se recomienda el uso de venv, se puede usar la extension en vscode o el comando
python -m venv nombre_del_entorno

Librerias
Puedes instalarse usando pip install -r requirements.txt

o bien 
pip install "stable-baselines3[extra]"
pip install tetris-gymnasium
pip install gymnasium[other]
en ese orden

Ademas para hacer funcionar CnnPolicy es necesario modificar RgbObservation dentro de testris-gymnasium
*carpeta_de_python*
    |_Lib
      |_site-packages
        |_tetris_gymnasium
          |_wrappers
            |_observation.py <-------

Aqui Cambiar self.observation_space la variable high a 255 en ves de tetrimonio



test push firebase studio