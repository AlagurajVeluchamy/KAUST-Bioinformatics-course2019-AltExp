Resource site: https://github.com/CBC-KAUST/AltExpKAUST2019

Terminal: ssh velucha@ilogin.ibex.kaust.edu.sa

Terminal: srun --time=5:00:00 --mem=16G --nodes=1 -c 16 --pty bash -l
Terminal: git clone https://github.com/CBC-KAUST/AltExpKAUST2019.git
Resource site: http://rnaseq-mats.sourceforge.net
Terminal: module load rmats/4.0.2
Terminal: python rmats.py --b1 b1.txt --b2 b2.txt --gtf gtfFile --od outDir -t readType --nthread nthread --readLength readLength --tstat tstat
Terminal: cd outputaltsp
Terminal: more fromGTF.RI.txt
plot number of events for the 5 categories: wc -l fromGTF.* | grep -v "novel"
send graph: alaguraj.veluchamy@kaust.edu.sa
