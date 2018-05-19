## ISOClassify: Classify the alternative splicing modules

Requirements
------------
1. Install Python 2.6.x or Python 2.7.x and corresponding versions of NumPy and
SciPy.
2. Add the Python directory to the $PATH environment variable.

Installation:
------------
The source code can be directly called from Python.

Usage:
--------------------------------

    $ python IsoClass.py input_module_def_file output_module_type_summary output_module_type
    
The examples of input files are available with the zipped source code.

Example:
--------------------------------
Test IsoClass on sample input:
Run IsoClass.py as below to test the module classification script.

    $ python IsoClass.py IsoExon.txt IsoClassSummary.txt IsoClass.txt

Input: The module defination file as outputed by the rMATS ISO module detection pipeline.

Output - IsoClassSummary.txt: Two-column output file that summaries the number of splicing modules in each type:
- Splicing Type: The type of the splicing module represented. The junction is represented by '-'. 
Each number is an exon. Alternative 3' or 5' forms of the exons are marked by 'A's.
Multiple junctions are split by ':'.
- Count: Count of the splicing type contained in IsoExon.

Output - IsoClass.txt : Two-column output file that contains the classification for each splicing module:
- ASM: ID of the splicing module.
- Splicing Type: The type of splicing modules as described in IsoClassSummary.

Contacts and bug reports
------------------------
Shihao Shen
shihao@ucla.edu

If you found a bug or mistake in this project, we would like to know about it.

This program is licensed with commercial restriction use license. Please see the attached LICENSE file for details.
