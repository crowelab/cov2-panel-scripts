# COV2 Panel Scripts
Scripts relating to the Rapid isolation and profiling of a diverse panel of human monoclonal antibodies targeting the SARS-CoV-2 spike protein manuscript


#### Organizing CDR3 lengths data

To generate the CDR3 distribution plots, feed in a list of CDR3 lengths that correspond to each sequence in the data set. Then run the Organizing Data-countingCDR3lengths.py script. This will count the number of entries with each CDR3 length. The output csv is then used as the input for the Plot CDR3 lengths.py

Example of input file: cdr3s.csv

#### Plot CDR3 lengths

To plot these histograms, open the output file from the script above, and make two new csv files. One for the heavy chain counts and one for the light chain counts. These will be the input file for the Plot CDR3 lengths.py script. 

Examples of these input files are heavy-cdr3-dist.csv and light-cdr3-dist.csv.

#### SHM Violin Plots

To plot the violin plots, use the script SHM_Plots_py.py. It takes a list of percent identity to germline values as a csv separately for the heavy chain and light chain. 

Examples of these input files are COV2-SHM-HC.csv and COV2-SHM-LC.csv.

#### VJ Heatmaps 

To plot the heatmaps use the script VHeatmaps.py. It takes a the zscore value of a V-J combination grid - separate for the heavy and light chains, and plots the zscores as a heat map. 

Examples of these inpuyt files are lambda.csv, kappa.csv, and heavy.csv. 

All the example files in this repo are similar to the ones used for the paper. 
