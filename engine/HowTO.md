If you just want to try the framework.
The simplest way is to deploy all the micro-services on a simple system and run the testcase.

(The default configure file is already set all the IPs to the local IP address.)

Following these steps:

```
git clone https://github.com/huawei-openlab/oct.git
cd oct/engine
make
cd testserver
./testserver &
cd ../ocitd
./ocitd &
cd ../containerpool
./containerpool &
cd ../scheduler

# choose a testcase.
./scheduler case01/Network-iperf.json

```
The raw result will be store at /tmp/test_scheduler_result/
