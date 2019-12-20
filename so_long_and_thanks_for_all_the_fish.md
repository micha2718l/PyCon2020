# Title
## So Long and Thanks for All the Fish: Listening to dolphins using Python and the scientific stack.

# Description
Dolphins are incredible animals who use audio for echolocation as well as communication. Come on a tour with me of building a data pipeline and analysis system for 10's of terabytes of audio data from under the Gulf of Mexico. The data engineering in nearly pure Python, the visualizations using matplotlib and Bokeh, and noise cleaning and analysis using NumPy, SciPy, and PyWavelets; all with a view into distributed systems. As well as a story of convincing an established team of scientists to move away from MatLab and to start using open source technology.

Ever been curious about how to compute a spectrogram? Or want to learn about some modern ways of building distributed computational systems? This talk will yield many tips and tricks to take back to your team or project. See the progression of using single Python scripts on small data to using Jupyter Notebooks for better presentation, all the way to scaling up to clusters of computers using Dask.

# Outline
- 0m:5m
    - The talk will start with a brief overview of how the project came to be and how our team obtained our data. Also covered is description of the state of the project when I joined, which included a lot of legacy MatLab code.
- 5m:10m
    - Moving beyond having data to work with, the next steps involved getting easy access to the data for myself as well as the rest of the team. The data is in a specific format and Python code was written to parse these files, and then some routines to work with it were added. This resulted in a Python package which now resides on PyPi. The experience of packaging and uploading for use with pip was enlightening.
- 10m:15m
    - Once the data is available, the next steps involve various ways of looking at the data. The audio is recorded at a very high sample rate, much higher than humans can hear. Here, I show how to do some simple plots to looks at the signals, as well as the basics of how to start digging into the frequency spectrum. Brief audio clips (slowed down for our inferior ears) will be presented to really get a feeling for what these creatures are doing.
- 15m:20m
    - Viewing small chunks of the data can be useful, but what is more interesting is to start looking at information across many hours or even days of audio. For this we will explore a few different parallel and distributed computing paradigms, and land on using Dask to do computation across compute nodes. This process is generally applicable to many different problem domains, and the work will be presented in a way that anyone should be able to apply small parallel improvements to almost any code.
- 20m:25m
    - Finally, we apply some machine learning techniques for clustering and labeling, even dipping into using NLP (the dolphins are really very smart, it is my opinion that they are saying some really interesting things). These results are presented with code examples and descriptions of how to apply some algorithm or technique which was not designed directly for the application but may yield interesting results anyway. This section will talk about the concept common in science, failures teach one more than any success ever will.
- 25m:30m
    - A conclusion will be made about the power of using open source scientific software, Python/NumPy/SciPy in particular. As well as a call to action for anyone interested in helping protect the creatures we share this world with; and a reassurance that these ideas and techniques are not beyond anyone with a basic knowledge of programming, or at least a desire to learn.
  
# Audience
The intended audience for this talk is first and foremost anyone interested in the wonderful world of dolphins and the conversations they are having. From a technical perspective, those at an intermediate level will learn the most details of how to work with large amounts of audio data, specifically in the realm of spectral analysis. From a Python perspective there should be ample tips and tricks that anyone from a beginner to expert should pick up something useful.

# Additional Notes