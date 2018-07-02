# frozen_sliders

An example of building a standalone bokeh application with pyinstaller.

    pyinstaller --onefile sliders.py

Based on one of the official bokeh examples: https://demo.bokehplots.com/apps/sliders

Works with master branch of bokeh (milestone 1.0).

Until `hook-bokeh.py` ([PR3607](https://github.com/pyinstaller/pyinstaller/pull/3607)) is merged into pyinstaller, it needs to be 
included manually:

    pyinstaller --additional-hooks-dir=. --onefile sliders.py 
