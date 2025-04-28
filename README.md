# Qscan
Code to perform Morlet-Gabor wavelet decomposition of LIGO data - a Qscan. Translated to python from original code by Neil Cornish.

To perform a Qscan:

1. Run the code LIGO_PSD.py which fetches the amplitude spectral density (sqrt(PSD)) and the FT of the data from LIGO. It writes and saves four files, two for each detector (labeled by 'H1/L1' for Hanford/Livingston, respectively). It runs in command line with: 'python LIGO_PSD.py 1126259460 4' where '1126259460' is the GPS start time and '4' is the duration you'd like to analyze (in seconds). The example given is the GPS time coresponding to GW140915.
2. Run 'doqscan.py', this will do the qscan for one of the detectors (currently Hanford) and can plot it or save it to file if you so want. It should be easy enough to modify to do both detectors in one go.

