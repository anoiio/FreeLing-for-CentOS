# FreeLing-for-CentOS
FreeLing compiled for CentOS with Java binding from [FreeLing master](https://github.com/TALP-UPC/freeling)

For licenses refer to [FreeLing web page](http://nlp.cs.upc.edu/freeling)


lib directory: includes FreeLing lib files compiled for CentOS 7 including Java binding library. 
reeling.jar: FreeLing Java API

## Installation:

1. Install dependent lib: yum install boost-devel
3. Copy lib directory to the desired location (e.g. /usr/local/lib)
4. Run script: lib/setLinks.sh
5. Set lib path: export LD_LIBRARY_PATH=<path_to_freeling_lib>
6. To use FreeLing API in your Java application include freeling.jar and load "freeling_javaAPI" system library (System.loadLibrary("freeling_javaAPI");).
7. In addition, data should be installed from the [FreeLing/data](https://github.com/TALP-UPC/FreeLing/tree/master/data)