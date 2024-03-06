# manualSiftMask()

This is an EEGLAB plugin to 
1 Show a butterfly plot of frequency-domain (i.e. time averaged time-frequency decomposed) dDTF08. 
2 Deteremine and apply statistical significance for a given single frequency bin.

How to use the function
1. Download the folder of this plugin from this site.
2. Go to the directory [eeglabroot]/eeglab/plugins
3. Paste the folder in this directry.
4. Re-launch EEGLAB.
5. 

When the plugin is successfully installed, you see the item 'Manual SIFT mask' under 'Tools'.
<img src="images/001.jpg" width="600" height="600">


Load a dataset with pre-computed dDTF results, then launch this plugin. Press 'Import SIFT data' button and you see the butterfly plot of time-averaged dDTF08 from all graph edges.
<img src="images/002.jpg" width="600" height="600">


Now you determine which frequency bin to analyze by sepcifying the frequency bin [Hz]. This adds a fine vertical red line to highlight the freq bin selected.
<img src="images/003.jpg" width="600" height="600">


Now you specify the cutoff p-values (the right-hand tail only for now). This p-value indicates deviation from zero (i.e. equivalent of one-sample t-test).
<img src="images/004.jpg" width="600" height="600">


Now you apply the selection by pressing the button 'Apply the mask and quit'. The graph edges that do not survive will be masked with zeros. This change cannot be redone. If you make a mistake, load the data again. Be careful not to overwrite existing data with the masked data!



03/06/2024 Makoto Miyakoshi.
