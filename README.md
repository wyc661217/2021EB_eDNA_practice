# 2021 E&B Practical Class on eDNA
This repository is for the bioinformatic section of environmental DNA (eDNA) practical class for the course NST Part IA: Evolution and Behaviour 2020-21. You will follow the guide step by step to experience how to process a shotgun sequencing dataset generated from a 46,000 years old permafrost sample from the Taymyr Peninsula of north Central Siberia. Before start, make sure you have watched the introduction vedio on moodle (https://www.vle.cam.ac.uk/course/view.php?id=203281&sectionid=3292581).

If you are familiar with the Linux system, you are also encouraged to run the processes by yourself, through it will take quite some time to process a real size sequencing dataset on your laptop. But this is optional. 

```
git clone https://github.com/SAMtools/htslib
git clone https://github.com/miwipe/ngsLCA
cd htslib
make
cd ../ngsLCA
make HTSSRC=../htslib
```
