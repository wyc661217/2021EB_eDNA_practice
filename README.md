# 2021 E&B Practical Class on eDNA

This repository is for the bioinformatic section of environmental DNA (eDNA) practical class for the course NST Part IA: Evolution and Behaviour 2020-21. You will follow the guide step by step to experience how to process a shotgun sequencing dataset generated from a 46,000 years old permafrost sample (sample ID ar1_2) from the Taymyr Peninsula of north Central Siberia. Before start, make sure you have watched the introduction vedio on moodle (https://www.vle.cam.ac.uk/course/view.php?id=203281&sectionid=3292581).

If you are familiar (or like to explore) the Linux, you are also encouraged to run the processes by yourself, through it will take quite some time to process a real size sequencing dataset on your laptop. You will be able to download the raw data in this link. But this is optional. 


## Data format

Usually when you submit a sample for sequencing, you will get a compressed file in fastq format, like ours "ar1_2.fastq.gz". Let's first decompress the file.

```
gzip -d ar1_2.fastq.gz
```

The above commond line runs a compressing program called "gzip" on our file "ar1_2.fastq.gz", and by stating "-d" we tell the program we want to decompress. After this we get a new file called "ar1_2.fastq", let's have a look into it.

```
less ar1_2.fastq
```

And you will see the inside the fasta format, there are millions of lines like this:

```
@K00234:90:HTWVHBBXX:7:1101:1793:1719 1:N:0:CGATGT+CGCTTG
TTGAGGTGCAACCCCCTACTCTTTCTCTGTTCATCTTTAACCAAATCGGAAGAGCACACGTCTGAACTCCAGTCACCGATG
+
AAFFFJJFAJAF---A-A--FFF-F--<F-FFAJFJFJJJF-<-AA<FJJJFFFJFJA7AJFA-7<AA7-AF<JJ-FJ-FA
@K00234:90:HTWVHBBXX:7:1101:2585:1719 1:N:0:CGATGT+CGCTTG
AAAAAATGAAGTCAGCAGAAAGGAAAGCACAAAATCACATTAAACTTTCAGAGATCGGAAGAGCACACGTCTGAACTCCAG
+
AAFFFJJJJJJJJJJJFJJJFJJFJJFJJJJJJFJJJJFJJJJJJJJJJJJFAJJJJJJJA<JJJJJJJJJJJJJFFJJJJ
@K00234:90:HTWVHBBXX:7:1101:1600:1736 1:N:0:CGATGT+CGCTTG
CGGTGTCACTTTGTCGGTATAGCCATCAATAATATTGATTTTGTCCAACTCTCTGGAAATAGATCGGAAGAGCACACGTCT
+
AAAFFJJJJJJJJJJJFJJJFJJJJJJAFFAFJ<JJJ<AJJJJJJJFFJJFJJJJJFFJAFFJJFFFJJFFF7JJJJJJJJ
@K00234:90:HTWVHBBXX:7:1101:1824:1736 1:N:0:CGATGT+CGCTTG
AATTTCGTGAACCAGCAAGTTGTTTGGTTGAAATATCTCGGTTTTGTTAGAATAGATACCGTAAGATTGTTCTAATCTATT
+
<A<-A<FJJJJFAJF-7FF<<F-7<AJFFF<-A<FJA-<7-----<7FFJ7JJJFJAJFJFFFF7JJJF--<<<AFJF<<A
```
Evry 4 lines compose a DNA sequence. The first line is the sequencing header, it always starts with a "@" and preserves basic information about the sequence. The 2nd line is our DNA sequence (we call it read in bioinformatics), normally formed by the 4 nucleobases A, T, C, and G. Followed with a "+" in the 3rd line and then the quility scores for each base of the read in the 4th line.


## Data qulity control

xxx

## Alignment

xxx

## Taxonomic classification

xxx












