# WARNING: This class assignment contains copyrighted material.

## Conventions pertaining to file management in project directory:
We've created **6 different jupyter notebook files**, each with the following purpose: 
- *Assignment_1* is the complete project file that contains code that corresponds to every question of the assignment, as well as two supplementary code cells in the beginning. These two code cells create two simple signals that can, alternatively, be passed as input to the 'librosa.load' function used in question A. This is the only purpose they serve, it's not mandatory to run them (even if user presses "Run all", it won't change anything codewise, as they are not used anywhere).
- *Assignment_1_A_C* contains code that corresponds to questions A and C of the assignment (since we're told that question B code should be placed in separate files, one for each subquestion).
- *B1, B2, B3 and B4* all contain code that corresponds to respective question B subquestion 1 - 4. 

Upon running either the "Assignment1.ipynb" or "Assignment_1_A_C.ipynb" file, the folder **Sound files** will be created in current directory. This is the folder that all our **GENERATED** sound files are placed by default. It's important to note the *generated* part. Oftentimes, in this assignment, we want to save signals we've created in this folder, for experimentation purposes. We've, also, placed some commented out quantization lines of code, in case user wants to replay audio file using Media Player (it doesn't support floating point values). All of this is **NOT** mandatory and it does not happen after every signal creation, only after some parts where we've played the signal (using the sounddevice module). Every line where we play the generated signal sound is commented out. Comment it in to hear what the generated signals sounds like (some parts contain volume factors to decrease the "volume" of generated signal).

There also are a lot of commented out print's throughout the code (in case you want to print out the peak frequencies, amplitude frequency pairs, etc.) in selected parts of some code cells.

You can also comment out every line that saves .wav files into the 'Sound files' folder (in case files are ran in Google Colab, kaggle, etc). It is also important to note that user can't have more than 3 runtimes simultaneously active in Google Colab, however this is not an issue when it comes to the execution of the B1, B2 and B3 script files.

**IMPORTANT NOTE**: We save our variables for script files B1, B2, B3 and B4 through pickle file 'variables.pickle'. If user decides to run this notebook file in Google Colab, kaggle, etc, they HAVE to download the file and re-upload it in session storage EVERY TIME they wish to run a new script. This is done to avoid mounting the file in Google Drive and encountering other issues pertaining to, mostly, permissions. This means that, if user runs 'B1.ipynb' in Colab, they should download the 'variables.pickle' file in their system and, when they open 'B2.ipynb', they should upload the file to session storage. Respectively, after B2's execution, they need to RE-DOWNLOAD the 'variables.pickle' file (since new variables were added), and so on.
