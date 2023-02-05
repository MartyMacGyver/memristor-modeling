# Memristor Modeling repo

**Includes a SPICE model suitable for use with LTspice**

By Martin Falatic (www.Falatic.com)

Except where otherwise noted, my contributions are licensed under the MIT license (see the LICENSE file for details).

Originally released via web 2013-01-10:

http://www.falatic.com/index.php/69/memristor-simulation-with-ltspice-a-practical-example

** These examples are provided for informational purposes ONLY. **
** No warranty is expressed or implied. **

I'd been curious about memristors for a while, and decided to see if I could
model one in LTspice (since I didn't find one there). This is the result.
This is not by any means definitive, just an example of the memristor as
described in one of the more well-known papers on the subject.

This was most recently tested successfully with LTspice64 17.1.6 (see install notes).

https://www.analog.com/en/design-center/design-tools-and-calculators/ltspice-simulator.html

Install the contents of the LTspice_model folder into the corresponding LTspice folders of your installation:

* For LTspice64 on Windows (should be similar for other platforms)
  * Install LTspice64 and browse to `%LOCALAPPDATA%\LTspice\lib`
  * Clone this repo and browse to `LTspice_model`
  * Copy the files from `lib\sub` and `lib\sym` to their respective LTspice `sub` and `sym` directories

Simulation:

* Open this `memristor_sim.asc`
* Select "Simulate" -> "Run"
* The output should match what you see in the `memristor_sim_example.png` file
* If the plot settings didn't load automatically:  
  * Click on the graph tab
  * Select "Plot Settings" -> "Open Plot Settings File"
  * Select `memristor_sim.plt`

Resources used:

* SPICE Model of Memristor with Nonlinear Dopant Drift (2009, Biolek, et. al.) (can be found at http://www.radioeng.cz/fulltexts/2009/09_02_210_214.pdf)
* Discussions on EDAboard (particularly http://www.edaboard.com/thread202648.html)
