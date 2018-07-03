# noncestatistics
a simple tool to get a bunch of ApNonces from iOS devices

Version: 97173d496566b63921e3377afc7b6018f3990671 - 1
Usage: noncestatistics [OPTIONS] FILE
tool to get a lot of nonces from various iOS devices/versions

  -h, --help             prints usage information
  -e, --ecid ECID        manually specify ECID of the device. Uses any device if not specified
  -t, --times amount     speficy how many NONCES are collected. If not specified it will collect nonces until you enter ctrl+c
  -a, --abort            resets device to normal mode
  -s, --statistics FILE  print statistics from nonce file
  FILE                   File to write nonces to

Examples:

Collect 500 ApNonces and write them inside nonces.txt:
        noncestatistics -t 500 nonces.txt

Do statistics on the nonces collected in nonces.txt
        noncestatistics -s nonces.txt


