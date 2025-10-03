On Vs code : 

Install the Extension : 
LaTeX Workshop 

Then :
Ctrl + S = save => automatic compilation
Ctrl + alt + V = put the compiled programm side by side with the associated code
Ctrl + alt + B = compile 

On Linux :

Install latexmk (Debian) :
sudo apt update
sudo apt install latexmk

latexmk -c => clear all unwanted files
latexmk -pdf yourfile.tex => generally used for the final compile
latexmk -pdf -pvc yourfile.tex => used for continus compile

