# EFDC+

The Environmental Fluid Dynamics Code Plus 8.5 (EFDC+ 8.5) is an enhanced version of the original EFDC code developed by John Hamrick.  EFDC+, previously referred to as EFDC_DSI, has undergone continual development and improvement over the last 20 years by DSI, LLC and collaborators such as Sandia National Labs, and USACE.  The EFDC+ code has been extensively utilized in hundreds of modeling studies.  It has evolved over the past two decades to become one of the most widely used and technically defensible hydrodynamic models in the world. 

 
EFDC+ is a state-of-the-art hydrodynamic model that can be used to simulate aquatic systems in one, two, and three dimensions.  It solves the three-dimensional, vertically hydrostatic, free surface, turbulent averaged equations of motion for a variable-density fluid.  Dynamically-coupled transport equations are also solved for turbulent kinetic energy, turbulent length scale and optional water column constituents including salinity, temperature, dye and others.  Unique EFDC+ features include drying and wetting in shallow areas by a mass conservation scheme and vegetation drag.  In addition to these features, EFDC+ is capable of simulating sediment transport with erosion and deposition, the transport and fate of hydrophobic toxic contaminants, eutrophication kinetics, Lagrangian particle tracking (LPT), and oil spill modeling. 


# Contents of this Repository

``EFDC`` - Contains all source code to build EFDC+ and executables for different build configurations

``NetCDFLib`` - Necessary library files for building EFDC+ to enable output into a NetCDF file format

``GridGenerator`` - Contains the executable for the simple Grid Generator for EFDC+

``GetEFDC`` - Contains source code for building utility that helps extract EFDC+ formatted binary time series data

``WASP`` - Provides files necessary for linkage with the WASP code (advanced used feature)

``SampleModels/`` - Contains several sample EFDC+ models

``docs`` - Contains documentation for EFDC+

The contents of each folder is described below:

	EFDC/ - 
		|-- DebugDP64/ 
			`-- *.dll
		|-- DebugSP/
			`-- *.dll
		|-- DebugSP64/
			`-- EFDC.exe
			`-- *.dll
		|-- ReleaseDP64/
			`--EFDC.exe
			`--*.dll
		|-- ReleaseSP/
			`-- EFDC.exe
			`-- *.dll
		|-- ReleaseSP64/
			`-- EFDC.exe
			`-- *.dll
		`-- *.f90

	NetCDFLib/
		|--	include/
			`-- C++ header files
		|--	lib/
			`-- *.lib 

	GridGenerator
		`--GridGenerator.exe
		`--	*.dll

	GetEFDC/
		|-- src/
			`-- *.f90

	WASP/
	
	SampleModels/
		|-- Ohio_River_4
		|-- Lake_T_HYR_WQ
		|-- Lake_Washington

	docs/ 
		|-- build/
			`--*.rst
		|-- gridgen/
			`--*.rst
		|-- images/
			`--*.rst
		|-- inputfiles/
			`--*.rst
		|-- outputfiles/
			`--*.rst
		|-- samplemodels/
			`--*.rst
		|-- started/
			`--*.rst
		|-- _images/
		`-- conf.py - Sets up configuration for Sphinx documentation builder
		`-- index.rst - Root RST file
		`-- license.rst
		
# License

Redistribution and use in source and binary forms, with or without modification, 
are permitted provided that the following conditions are met:

     Redistributions of source code must retain this list of conditions and the 
     following disclaimer.
  
     Redistributions in binary form must reproduce this list of conditions and 
     the following disclaimer in the documentation and/or other materials 
     provided with the distribution.
  
     Neither the name of the U.S. Environmental Protection Agency nor any other 
     contributors may be used to endorse or promote products derived from this 
     software without specific prior written permission. 

THIS SOFTWARE IS PROVIDED ``AS IS'' AND ANY EXPRESS OR IMPLIED 
WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED 
WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR 
PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE U.S. ENVIRONMENTAL 
PROTECTION AGENCY OR OTHER CONTRIBUTORS BE LIABLE FOR ANY DIRECT, 
INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL 
DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF 
SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR 
BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF 
LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT 
(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF 
THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF 
SUCH DAMAGE.