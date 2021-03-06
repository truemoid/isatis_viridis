# Viridis colour palette for Isatis #

The Python 2D plotting library [matplotlib](http://matplotlib.org/) changed its default colour palette from a rainbow-based scheme called jet to a new scheme called viridis. Viridis was designed to be:

- *Perceptually uniform*: no particular colour stands out more than any other. This is important in scientific visualization to prevent artificial patterns or trends appearing in the data because one colour is more apparent to the human eye than another.
- *Printable in grey-scale*: if the colour palette happens to be presented, printed, or photocopied in grey-scale the highs and lows can still be identified. It is perceptually uniform in grey-scale as it is in colour.
- *Colour blind compatible*: people with the most common forms of colour blindness should still be able to interpret visualizations using this colour palette.

In these three areas the new palette is superior to traditional rainbow-based palettes. You can read more about [viridis](http://bids.github.io/colormap/) or watch the [presentation](https://youtu.be/xAoljeRJ3lU), which has an interesting discussion of the theory.

I have created a series of viridis palettes for [Isatis](http://www.geovariances.com/). There are several palettes with different amounts of colour levels (some Isatis processes may have difficultly with high numbers of levels). The 128-level palette should work in most instances but switch to 64 or 32-level palettes if you have trouble.

During the development of viridis three other colour scales were developed that have a warmer appearance. I have included palettes for these three scales: inferno, magama, and plasma.

<img src="https://github.com/politiken-journalism/scale-color-perceptual/blob/master/example/example.png?raw=true" alt="Inferno, magma, plasma, and viridis, respectively (from politiken-journalism)" width="500px">

**Inferno, magma, plasma, and viridis, respectively** -- from [politiken-journalism](https://github.com/politiken-journalism/scale-color-perceptual.git)

The palette files are in the text file export format used by Isatis. To import the palette go to `File->Color palettes...` and select `Import...` to import the ASCII file. You can now create viridis-based colour scales for visualising data. Alternatively run the journal file included in this repository ([journals folder](https://github.com/amt4158/isatis_viridis/tree/master/journals)) making sure that you modify the path variable.

I have also included an R script for generating the colour scales in case you would like to modify what I have done. This script is a bit of a hack based on the work of Simon Garnier (and others), who created the [viridis package](https://github.com/sjmgarnier/viridis.git) for R.

If you are acustomed to using rainbow colour palettes it can take a bit of getting used to a palette like viridis; however, I think after a while you will agree that it is superior.
