
# dRepanalyzer

![dRepanalyzer_logo](https://github.com/AleksG98/dRepanalyzer/assets/135729246/20108035-b00a-409b-824e-8b7da12d957a)


<details>
<summary>Disclaimer</summary>

This script is a project developed by students of a Molecular Biology Master's Programme at the University of Padova, during the lab classes in course Microbial Metagenomics. The project was developed under the supervision of Prof. Stefano Campanaro.

</details>


dRepanalyzer is a tool that can compute a resampling procedure and produce a rarefraction plot based on input files produced by dRep and CheckM softwares.
The objective of this script is to produce a rarefraction plot which underlines the abundance of samples needed to dissect the microbial environment structure.

## Requirements

Requirements to run this script are: The software was developed based on python 3.10. It requires several common libraries. To discover if a system has the right requirements, run -check_dependencies.

## Inputs

In order to run dRepanalyzer, the output of two softwares is used: dRep and CheckM. As an output of dRep software, one of the files received is Cbd.csv, which shows the assignment of the genomes to the clusters. For each genome the table returns secondary clustering results based on the default threshold, together with additional information. CheckM software generates a table providing for each genome bin identified (+ a line for unbinned contigs) the bin Id, the bin size (Mbp) and 4 different relative abundance measures, repeated in series as many times as the samples employed for the analysis. 

## How to run the software

The software is provided as an executable file. From the working directory, in the command line you can check how to run the software and an example by running:

```
dRepanalyzer
```

or

```
dRepanalyzer --help
```

In order to check whether all required libraries are installed, you can run:

```
dRepanalyzer -check_dependencies 
```

In case you are missing some libraries, it will raise an error showing which libraries are yet to be installed.

## What are the outputs

As a result of running the software, you get two types of files:

*  **.pdf** containing the rarefraction plot
*  **.res** contanining the results of the resampling processes in a tabular format













