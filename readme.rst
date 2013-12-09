========
The List
========

Human Motion and Control Lab
============================

- Write up walking database proposal
- Write blog post about all of the tours we've given
- Setup the NAS server

Gait Control System Identification
----------------------------------

- Finish reading the van der Kooij paper

  - Section 2
  - Section 3
  - Section 4

- See if our controller can drive an OpenSim model or Ton's 2D model

  - Investigate the 2D models in Open Sim
  - Reproduce the sample controller that is in OpenSimm

- Wrap Ton's walking model from his tutorial

  - Go through "Learn C the Hard Way" to get back up to speed in the
    language

    - Exercise 14
    - Exercise 15
    - Exercise 16

  - Read about MEX functions in Matlab
  - Try using SWIG for Matlab/Octave wrapping

- Create Ton's gait2de model with PyDy
- Organize Ton's gait2de code and include my PyDy code for public distribution.

- Wrap the HBM C code

  - try out the cython wrapping I started, need the source for hbm or a
    shared library though

- Test out running with perturbations on the treadmill
- Do we need to prevent the subject from seeing the treadmill
- Do we need a white noise thing for the subject to watch on the screen

Lab Website
-----------

- Enable MathJax the "correct" way
- Duplicate website backups offsite (on our NAS or S3 bucket)
- Complete the Diazo rules in the theme and upload to the website
- Add all the buttons I've clicked to the generic settings and push to live
  server
- Setup workflow for website for publishing public documents
- Investigate ways to display publication lists on the website

  - check into embedding zotero collections into a page
  - check into using CMFBibliographyAT with Plone 4.3

- Get folks to submit headshot and bio: need Samin
- Finish the a people page: need Samin
- Figure out how to display the event date instead of the creation date in
  the rss feed: https://github.com/csu-hmc/hmc.csuohio.edu/issues/1
- Overload the rss portlet template to get the gcal event data instead.
- Add google analytics.
- Allow anonymous commenting.
- Make an internal reviewer role that has all permissions of a reviewer except
  approving external publication. Use this for the lab doc folder. Another
  solution would be to have a specific workflow for that folder (i.e. no public
  parts and the lab has full access to the folder.)

Yeadon
======

PLoS One Paper
--------------

- Review the TODO items on the Yeadon paper
- Finish the bicycle configuration example

Bicycle Stuff
=============

- Find info about bicycle Simulator by Hattori in Japan before 1973.
- Write up a project description for measuring ground reaction forces of the
  gyrobike
- Upload all experimental data to figshare (videos, raw data, HDF5 file)
- Make a HDF5 file of the raw data plus the unfiltered processed data and
  upload to figshare.

  - Write a script that bundles the BicycleDAQ .mat files into several zipped
    tar balls.
  - Write a script which uncompresses the BicycleDAQ data back into the correct
    directory structure.
  - Upload BicycleDAQ data to FigShare. This should probably include the
    corruption csv file too.
  - Write a script that bundles the video files of the instrumented bicycle
    into several <250 mb zipped tar balls. Also write the script to unbundle.
    them. Upload to figshare.
  - Generate an H5 file with just the raw data tables
  - Generate an H5 file with the raw data and unfiltered processed data for as
    many runs as possible.
  - Make a DOI for the H5 files but only include a readme that points to a
    download on my site.

Whipple ID Paper
----------------

  - Add how to download data and cleanup instructions to run everything.
  - Include source code for generating the mean VAF table (this will be a bitch
    because it relies on matlab). Could try to write this in Python.

Steer torque paper
------------------

  - Add how to download data and cleanup instructions to run everything.
  - Use the static data testing data to verify steer torque compensation works
    (would be nice if I had some no-hands data)
  - Find out more details about Kondo/Kagyema measurements of steer torque

BMD 2013
--------

- Post update on my blog about BMD/JSAE copyright conclusion

PyDy/SymPy
==========

- Start proposal for PyDy future

   - http://www.multibody.net/mbsymba/ add to proposal

- Try out CSympy with some mechanics problems

  - Build cysmpy
  - Replace appropriate imports with csympy functions in mechanics
  - Compare the n-link pendulum derivation speed problem speed with/without csympy

PyDyViz
-------

- Push pydy_viz release 0.1.0 to PyPi
- Review Tarun's tutorial PR(s)

- Make some example visualizations
- Speed up the transform generations in pydy viz
