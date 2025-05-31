# TimedTraceAlignment Tool

## Overview
TimedTraceAlignment takes as input a process log, specified in the XES (eXtensible Event Stream) format, and a set of declarative constraints expressed using the Timed Declare language (.decl file). The tool outputs the problem in PDDL, which can be directly executed using the [ENHSP planner](https://sites.google.com/view/enhsp/).

## Prerequisites
Before using the TimedTraceAlignment tool, ensure you have the following installed:

1. **Python 3.x**  
   Make sure Python 3.x is installed on your machine.

2. **ENHSP Package**  
   Download and install the ENHSP20 package from the [ENHSP Official Website](https://sites.google.com/view/enhsp/).  
   Follow the installation instructions provided on the website.

## Installation and Launch

The TimedTraceAlignment tool is executed via the command line, providing several options to customize the input and control how the alignment is performed.
The script is invoked using the following options:

- **log**: Specifies the path to the XES log file containing the process traces. This file is essential as it contains the sequences of activities that will be aligned. The file must conform to the XES (eXtensible Event Stream) standard.
- **decl**: Defines the path to the DECL (Declare) file that contains the temporal constraints and rules.

```bash
Example Usage:
python main.py -log example_log.xes -decl example_constraints.decl
```

