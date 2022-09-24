# compressed_spectral_array

We use compressed spectral array (CSA) as a representation of the resting-state electroencephalogram (rs-EEG) data.
Thus, CSA shows super-imposing linear plots of successive epochs of time on each other. The latter generates a 3-dimensional ‘hill and valley’ display of the power density in a single channel. 
Of note, as successive epochs are added to the display, information can become hidden behind ‘hills’ of increased power at particular frequencies [1].

In order to overcome the above limitation, an ```alpha=0.5``` transparency parameter, as well as a  ```t = np.sqrt(abs(delta))/1.5``` tuning parameter allow to control the height of the peaks.

This Jupyter Notebook includes an implementation of [Luc Kuster's Matplotlib-based waterfall plot](https://github.com/ljbkusters/mpl-waterfall-plot) adapted by [@yjmantilla](https://github.com/yjmantilla/) and [@alberto-jj](https://github.com/alberto-jj/) for EEG data. 

CSA can be plotted in B&W as well as using matplotlib colormaps
![image](https://user-images.githubusercontent.com/71186117/192097144-fa32ec1b-f83b-4bef-88a8-c07f36927845.png)
![image](https://user-images.githubusercontent.com/71186117/192097199-3f20ef55-70cd-4d84-a0b2-de9770310067.png)



[1] Whyte SD, Booker PD. Monitoring depth of anaesthesia by EEG. British Journal of Anaesthesia. 2003; 3(4): 103-10.
