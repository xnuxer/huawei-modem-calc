# Repository huawei-modem-calc

How to compile:

g++ huaweicalc.cpp -L/usr/lib -lssl -lcrypto -o huaweicalc

How to use:

./huaweicalc \<IMEI\>

# Example from console

<pre>
xnuxer@ubuntu:~$ g++ huaweicalc.cpp -L/usr/lib -lssl -lcrypto -o huaweicalc
huaweicalc.cpp: In function âint main(int, char**)â:
huaweicalc.cpp:56:50: warning: deprecated conversion from string constant to âchar*â [-Wwrite-strings]
     encrypt_v1(imeibuf, codebuf, "hwe620datacard");
                                                  ^
huaweicalc.cpp:59:47: warning: deprecated conversion from string constant to âchar*â [-Wwrite-strings]
     encrypt_v1(imeibuf, codebuf, "e630upgrade");
                                               ^
xnuxer@ubuntu:~$ ./huaweicalc 
usage: huaweicalc <IMEI>
xnuxer@ubuntu:~$ 
xnuxer@ubuntu:~$ ./huaweicalc 867648011803309
  IMEI              = 867648011803309
  Unlock code       = 34560983
  Flash code        = 34591526

</pre>
