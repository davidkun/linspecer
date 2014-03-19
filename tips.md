### Some tips for using linspecer ###
---------------------------------

I personally like the first color to be black, so I begin with:

	colors = [0,0,0; linspecer(10)];

which creates an 11x3 matrix of RGB colors.

Note: you must add the linspecer to your path via:

	addpath('~\path-to-linspecer-directory/linspecer')

you can add this to the startup.m file, found in your default startup directory for Matlab (on my Mac it's at `/Users/USERNAME/Documents/MATLAB/`)

If you'd like Matlab to use this color order by default, add this code to your startup.m file:

	addpath('~/path-to-linspecer/linspecer')
	colors = [0,0,0; linspecer(8)];
	set(0,'DefaultAxesColorOrder',colors);

where `'~/path-to-linspecer/linspecer'` is the path to you `linspecer` folder.
