# Introduction
Ligate is a Perl script that can merge several individual 3D RNA motifs within a PDB file into a single RNA structure. The script was developed to help design the single-stranded RNA origami structures published in Science in 2014 (http://science.sciencemag.org/content/345/6198/799.full). A protocol describing the details of the RNA origami design process has also been published (https://link.springer.com/protocol/10.1007%2F978-1-4939-6454-3_5).
# Usage
## Installing
Make sure you have a Perl compiler installed for your platform. Run the command `perl -version` in the command line to check for installed versions. If no installed versions are found, get an installer for you platform from https://www.perl.org/get.html.

Get the source files by running:
```
git pull git@gitlab.au.dk:esa-lab/ligate.git
```
## Running
Enter the source folder and ligate a merged PDB file. The script is run with the command:
```
perl ligate.pl inputfile.pdb > outputfile.pdb
```
Example files from the protocol mentioned in the introduction can be found in the "examples" folder. Ligate the file "4_2H-AE_merged.pdb" with the command:
```
perl ligate.pl 4_2H-AE_merged.pdb > 5_2H-AE_ligated.pdb
```
The file "5_2H-AE_ligated.pdb" should now be created by the script, and contain the ligated structure.
