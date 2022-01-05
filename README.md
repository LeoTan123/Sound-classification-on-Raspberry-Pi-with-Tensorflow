# SOUND CLASSIFICATION WITH TENSORFLOW ON RASPBERRY PI

![alt text](https://raw.githubusercontent.com/GianlucaPaolocci/Sound-classification-on-Raspberry-Pi-with-Tensorflow/master/img/Immagine.png)

##  BUILD THE PROJECT

  ~~The project is developed and tested with Python 2.7.~~ <br>
  The project has been updated to work with Python 3.7.

  ### Required Packages
  - TensorFlow (1.14.0)
  - Scikit-learn
  - Librosa
  - Sounddevice

  ### Installation on PC (PyCharm)
  1. Use PyCharm to create a new virtual environment
  2. Search and install the required libraries mentioned above
  
  ### Installation on Raspberry Pi
  1. Install numpy globally: <br>
  `sudo apt-get install python3-numpy`


  2. Install scipy globally: <br>
  `sudo apt-get install python3-scipy` <br>
  *Note: `pip3 install -U scikit-learn` doesn't work


  3. Create a virtual env: <br>
  `python3 -m venv ac-env`


  4. Activate the virtual env: <br>
  `source ac-env/bin/activate`


  5. Allow venv to see all global packages using the system-site-packages option: <br>
  `virtualenv --system-site-packages -p python3 ./ac-env`


  6. Install TensorFlow: <br>
  `pip3 install tensorflow`


  7. Install Librosa: <br>
  `sudo apt-get install llvm` <br>
  `LLVM_CONFIG=/usr/bin/llvm-config pip3 install llvmlite==0.32` <br>
  `#pip3 install numpy` <br>
  `pip3 install numba==0.49` <br>
  `pip3 install librosa`


  8. Install sounddevice: <br>
  `sudo apt-get install libportaudio2` <br>
  `sudo apt-get install libatlas-base-dev` <br>
  `pip3 install sounddevice`
  
### Steps
1. **DOWNLOAD UrbanSound8K DATASET**

  https://serv.cusp.nyu.edu/projects/urbansounddataset/urbansound8k.html

2. **TRAIN THE MODEL**

  Set the right path where you downloaded the dataset in your code.

  Set the right path where you want to save the trained model.

  Run "trainModel.py" on your PC/Workstation.

3. **RUN THE MODEL**

  Export the trained model on you Raspberry Pi ('model.meta', 'model.index', 'checkpoint', 'model.data-00000-of-00001').
  
  Export 'fit_params.npy' on your Raspberry Pi.

  Run "classiPi.py" on your Raspberry and enjoy!

# REMEMBER TO

  Remember to reference this project in your works.

# AUTHORS
 
  Gianluca Paolocci, University of Naples Parthenope, Science and Techonlogies Departement, Ms.c Applied Computer Science
  https://www.linkedin.com/in/gianluca-paolocci-a19678b6/
  
  Luigi Russo, University of Naples Parthenope, Science and Techonlogies Departement, Ms.c Applied Computer Science
  
# CONTACTS

  if you have problems, questions, ideas or suggestions, please contact me to:
  - **gianluca.paolocci@studenti.uniparthenope.it**
  
 <a href="http://www.reliablecounter.com" target="_blank"><img src="http://www.reliablecounter.com/count.php?page=https://github.com/GianlucaPaolocci/Sound-classification-on-Raspberry-Pi-with-Tensorflow&digit=style/plain/29/&reloads=1" alt="" title="" border="0"></a><br /><a href="http://" target="_blank" style="font-family: Geneva, Arial; font-size: 9px; color: #330010; text-decoration: none;"></a>


