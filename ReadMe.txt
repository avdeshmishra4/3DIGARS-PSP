Note: Before Running the Program
A large file under 3DIGARS-PSP\3DIGARS3.0\REGAd3p\Software\Models\SS_SVM\SSD_TR1001.libsvm.scale.model was splitted using winzip in 25MB size multiple files.
You may use winzip to merge the files with names SSD_TR1001.libsvm.scale.model.z01 to SSD_TR1001.libsvm.scale.model.z16 into a single file and make the merged large file is named as "SSD_TR1001.libsvm.scale.model" then run the program.


In this version the beta condition is verified and then the ssFreq table is used to get the best beta sheet ss type and the corresponding phi and psi angle.
This phi and psi angle is then used to replace the phi and psi at mutation point or the crossover point.

Compile: mpiCC *.cpp -o main.exe -lm
Run: mpirun -np 2 ./main.exe > console.txt

Note: This program uses Scwrl4 and 3DIGARS3.0 energy function. The 3DIGARS3.0 energy function internally uses REGAD3p method. The 3DIGARS3.0
	  and REGAD3p methods are modified for the smooth integration to 3DIGARS-PSP.
