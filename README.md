# Memristor Modeling repo
**(including model for use with LTspice)**

By Martin Falatic (www.Falatic.com)

Originally released via web 2013-01-10:
http://www.falatic.com/index.php/69/memristor-simulation-with-ltspice-a-practical-example

** These examples are provided for informational purposes ONLY. **
** No warranty is expressed or implied. **

I've been curious about memristors for a while, and decided to see if I could
model one in LTspice (since I didn't find one there). This is the result.
This is not by any means definitive, just an example of the memristor as
described in one of the more well-known papers on the subject.

This was most recently tested successfully with LTspice IV 4.23i
http://www.linear.com/designtools/software/#LTspice

I installed this as follows, where %LTINSTALL% = the install path (e.g. "C:\Program Files\LTS\LTspiceIV")

    Memristor_sim.asc -> %LTINSTALL%\
    Memristor_sim.plt -> %LTINSTALL%\
    memristor.asy     -> %LTINSTALL%\lib\sym\
    memristor.sub     -> %LTINSTALL%\lib\sub\

Simulation:
* Open Memristor_sim.asc
* Select "Simulate" -> "Run"
* Click on the graph tab
* Select "Plot Settings" -> "Open Plot Settings File"
* Select Memristor_sim.plt
* This output should match what you see in the Memristor_sim_example.png file

Resources:
* SPICE Model of Memristor with Nonlinear Dopant Drift (2009, Biolek, et. al.) (can be found at http://www.radioeng.cz/fulltexts/2009/09_02_210_214.pdf)
* Discussions on EDAboard (particularly http://www.edaboard.com/thread202648.html)
