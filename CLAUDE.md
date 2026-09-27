# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

soundscape implements a simple "audiolisation" function in python.
It tracks the position of the pointer on a graphics tablet or touch
screen, converts this position into a coordinate in a two-dimensional
array, then uses the array value in a lookup table for precomputed
samples at different frequencies which it plays. Thus the user can
scan through the array to hear the overall structure. It has zoom in
and out capability as well as the ability to print the array value in
response to key presses.
## Commands

```bash
# Enable environment
conda activate 3.11
```python
import soundscape
import numpy
t = numpy.arange(100).reshape((10,10))
soundscape.soundscape(t)
```

