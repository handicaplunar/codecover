# codecover
Python code coverage module to find the code coverage of products.

Structure of code:

Bin/
   / tests/*        test for the code
   /codecover.py    starting main function
   /readme          information file
   /setup.py        setup information
   /requirements.txt  requirement information
   
Bin/tag/                  *tag the code of which the code coverage to be done.
       /logger_mode.py    keep logging related function and variables
       /log_msg_gen.py    generate the log messages to be appended to the code.
       /indentation.py    get the indentation information of the code.
       /parsefile.py      parse the code file and generate the tagged code.
       
Bin/Mapping
      /get_msg.py         get message from tagging module and parse it.
      /create_map.py      create the mapping file from the logged messages.

Bin/Report
      /map_log.py         parse mapping and log file.
      /generate_report.py ceate a report based on parsed file.
      /calc_coverage.py   calculate coverage based on the report.
      /generate_files.py  generate output files for coverage report.
