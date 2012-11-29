check_tftp
==========

TFTP nagios check written in Python


```
Usage: check_tftp [options]

Options:
  -h, --help            show this help message and exit
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



Demo Run
--------
```
$ check_tftp -H tftp.example.com \
        -f linux-install/pxelinux.0 \
        -f linux-install/vesamenu.c32 \
        -f linux-install/logo.png \
        -l
OK: tftp://tftp.example.com/linux-install/pxelinux.0 got 89418B in 1.00 secs
tftp://tftp.example.com/linux-install/vesamenu.c32 got 155792B in 1.00 secs
tftp://tftp.example.com/linux-install/logo.png got 30487B in 1.00 secs | 'linux-install/pxelinux.0_size'=89418;;;; 'linux-install/pxelinux.0_fetch'=1.00337505341;;;; 'linux-install/vesamenu.c32_size'=155792;;;; 'linux-install/vesamenu.c32_fetch'=1.00353980064;;;; 'linux-install/logo.png_size'=30487;;;; 'linux-install/logo.png_fetch'=1.00428891182;;;;
```
