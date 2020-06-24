You can play Connect Four against this engine.

For positions at and below 9 ply, the engine may communicate with a DB (via SQLite) to evaluate them and find a good move. This DB was generated by a previous version of the engine (V.41) that thought on each reachable 9 ply position, and then these results were used to generate data for all 0 to 8 ply positions as well.

The file was too large to upload to Github, but it can be downloaded here:

https://drive.google.com/file/d/1f0q-X5edDGx_Rh-TuJIHSRoRlc2R1WED/view?usp=sharing

After downloading, copy this DB file to some directory on your computer.

After doing this, go inside the Version 50/bin/Debug directory, and then there are two options for setting up the pygame application.
Because of the size I couldn't directly upload it here.

  1) Open the command prompt and go to /bin/Debug. If you don't have pyinstaller, install it with "pip install pyinstaller".
     Then type "pyinstaller interface.py" - we're only interested in the dist/interface directory that gets created.
     In /bin/Debug, copy the following files (and paste them into /dist/interface): 
     directory.txt, error_effect.wav, move_effect.wav, OngoingScore.txt, second_move_effect.wav, signal.txt, and
     Version 1 - April 25, 2018.exe.
     
  2) Or, you can download the dist folder here: https://drive.google.com/drive/folders/1Sg3ngdTuro5F_YEK4QJoyHagDNzXj1Ud?usp=sharing
  
 After doing either of these options, go into /dist/interface, and open up the directory.txt file. Replace the line in it with the absolute
 directory of where you downloaded the database on to your computer.
 
 Finally, run interface.exe.
