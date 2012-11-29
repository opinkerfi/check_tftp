check_tftp
==========

TFTP nagios check written in Python


```
Usage: check_tftp [options]

Options:
  -h, --help            show this help message and exit
  -m MINSIZE, --minsize=MINSIZE
                        Minumum size of file
  -f FILE, --file=FILE  Remote file, use often for many files
  -w WARNING, --warning=WARNING
                        Warn if tftp downloads take longer
  -c CRITICAL, --critical=CRITICAL
                        Critical if tftp downloads take longer
  -l, --longoutput      Each file broken up into a new line for readability
  -v VERBOSE, --verbose=VERBOSE
                        Verbosity Level
  -H HOST, --host=HOST  Target Host
  -t TIMEOUT, --timeout=TIMEOUT
                        Connection Timeout

```
