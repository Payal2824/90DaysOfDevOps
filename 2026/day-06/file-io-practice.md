# linux file read / write practice

## command 
1.create file :- touch notes.txt

2.append the data on file :- echo "this is the 1st line" > notes.txt (> overwrite)

3.append the data on file :- echo "this is the 2nd line " >> notes.txt (>> append )

4.append the data on file using tee :- echo "this is 3rd line " | tee -a notes.txt 

5. read all data on file :- cat notes.txt
   
6.read data from first 2 lines :- head -n 2 notes.txt

7.read data drom last two lines :-  tail -n 2 notes.txt
