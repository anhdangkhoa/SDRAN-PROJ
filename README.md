## Code modification to export metrics_stdout to csv file in srsRAN
### Replace the orginal files in srsRAN with the files in this repogistory
    $ cp metrics_stdout.cc {srsRAN dir}/srsenb/src/metrics_stdout.cc
    $ cp metrics_stdout.h {srsRAN dir}/srsenb/hdr/metrics_stdout.h
### Recompile srsRAN to apply new code
    $ cd {srsRAN dir}/build
    $ make
    $ sudo make install

### The csv file will be save at `/tmp/enb_metrics.csv`
