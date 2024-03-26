openairinterface5


./build_oai --phy_simulators
```
> Returns
```
...
cd /home/bricer/Developer/openairinterface5g/cmake_targets/ran_build/build
Running "cmake3 --build .  --target dlsim ulsim ldpctest polartest smallblocktest nr_pbchsim nr_dlschsim nr_ulschsim nr_dlsim nr_ulsim nr_pucchsim nr_prachsim params_libconfig coding rfsimulator dfts -- -j28" 
Log file for compilation is being written to: /home/bricer/Developer/openairinterface5g/cmake_targets/log/all.txt
dlsim ulsim ldpctest polartest smallblocktest nr_pbchsim nr_dlschsim nr_ulschsim nr_dlsim nr_ulsim nr_pucchsim nr_prachsim params_libconfig coding rfsimulator dfts compiled
BUILD SHOULD BE SUCCESSFUL
```

```
cd ran_build/build
```

```
./nr_ulsim -C 4 -m 25 -s 24 -z 4 -n 100 -P -q 1 -R 273 -r 273
```
> Returns
```powershell
CMDLINE: "./nr_ulsim" "-C" "4" "-m" "25" "-s" "24" "-z" "4" "-n" "100" "-P" "-q" "1" "-R" "273" "-r" "273"
[CONFIG] get parameters from cmdline [CONFIG] debug flags: 0x00400000
Initializing random number generator, seed 13837415079507951325
handling optarg C
handling optarg m
handling optarg s
Setting SNR0 to 24.000000
handling optarg z
handling optarg n
handling optarg P
handling optarg q
handling optarg R
handling optarg r
[CONFIG] log_config: 2/3 parameters successfully set
[CONFIG] log_config: 50/50 parameters successfully set
[CONFIG] log_config: 50/50 parameters successfully set
[CONFIG] log_config: 16/16 parameters successfully set
[CONFIG] log_config: 16/16 parameters successfully set
log init done
create a thread for core -1
Assertion (ret == 0) failed!
In threadCreate() /home/bricer/Developer/openairinterface5g/common/utils/system.c:266
Error in pthread_create(): ret: 1, errno: 0
Exiting execution
Exiting at: /home/bricer/Developer/openairinterface5g/common/utils/system.c:266 threadCreate(), _Assert_Exit_
```




---


```
git clone git@gitlab.eurecom.fr:oai/openairinterface5g.git
```

```
cd openairinterface5g/cmake_targets
./build_oai --ninja -I 
./build_oai --ninja -P
```


# References

- [ ] [How To Install Ubuntu 22.10 On M1 or M2 Mac || RUN NEW Ubuntu On ANY Mac W/ Apple Silicon Using UTM](https://www.youtube.com/watch?v=O19mv1pe76M&t=0s)
- [ ] [oaiworkshop/summerworkshop2023/Repository](https://gitlab.eurecom.fr/oaiworkshop/summerworkshop2023/-/tree/main/ran)
