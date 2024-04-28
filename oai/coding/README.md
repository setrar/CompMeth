

- [ ] Removing code from 154-459

```powershell
/home/bricer/Developer/openairinterface5g/openair1/PHY/NR_ESTIMATION/nr_ul_channel_estimation.c:89:13: warning: unused variable ‘nushift’ [-Wunused-variable]
   89 |   const int nushift = (p >> 1) & 1;
      |             ^~~~~~~
/home/bricer/Developer/openairinterface5g/openair1/PHY/NR_ESTIMATION/nr_ul_channel_estimation.c:86:11: warning: unused variable ‘ul_ch_estimates’ [-Wunused-variable]
   86 |   c16_t **ul_ch_estimates = (c16_t **)pusch_vars->ul_ch_estimates;
      |           ^~~~~~~~~~~~~~~
/home/bricer/Developer/openairinterface5g/openair1/PHY/NR_ESTIMATION/nr_ul_channel_estimation.c:79:13: warning: unused variable ‘chest_freq’ [-Wunused-variable]
   79 |   const int chest_freq = gNB->chest_freq;
      |             ^~~~~~~~~~
[100%] Linking C static library libPHY_NR.a
WARNING: 3 warnings. See /home/bricer/Developer/openairinterface5g/cmake_targets/log/all.txt
```

```
cmake_targets/build_oai --phy_simulators
```
> Returns
```powershell
Will compile dlsim, ulsim, ...
OPENAIR_DIR    = /home/bricer/Developer/robert/openairinterface5g
Running "cmake3 ../../.."
-- Ccache not found. Consider installing it for faster compilation. Command: sudo apt/dnf install ccache
-- Check if /opt/asn1c/bin/asn1c supports -gen-APER
-- Check if /opt/asn1c/bin/asn1c supports -no-gen-UPER
-- Check if /opt/asn1c/bin/asn1c supports -no-gen-JER
-- Check if /opt/asn1c/bin/asn1c supports -no-gen-BER
-- Check if /opt/asn1c/bin/asn1c supports -no-gen-OER
-- CMAKE_BUILD_TYPE is RelWithDebInfo
-- CPU architecture is x86_64
-- AVX512 intrinsics are ON
-- AVX2 intrinsics are ON
-- Selected E2AP_VERSION: E2AP_V2
-- Selected KPM Version: KPM_V2_03
-- No Support for Aerial
-- No Doxygen documentation requested
-- Configuring done
-- Generating done
-- Build files have been written to: /home/bricer/Developer/robert/openairinterface5g/cmake_targets/ran_build/build
cd /home/bricer/Developer/robert/openairinterface5g/cmake_targets/ran_build/build
Running "cmake3 --build .  --target dlsim ulsim ldpctest polartest smallblocktest nr_pbchsim nr_dlschsim nr_ulschsim nr_dlsim nr_ulsim nr_pucchsim nr_prachsim nr_psbchsim params_libconfig coding rfsimulator dfts -- -j28" 
Log file for compilation is being written to: /home/bricer/Developer/robert/openairinterface5g/cmake_targets/log/all.txt
/home/bricer/Developer/robert/openairinterface5g/openair1/PHY/NR_ESTIMATION/nr_ul_channel_estimation.c:89:13: warning: unused variable ‘nushift’ [-Wunused-variable]
   89 |   const int nushift = (p >> 1) & 1;
      |             ^~~~~~~
/home/bricer/Developer/robert/openairinterface5g/openair1/PHY/NR_ESTIMATION/nr_ul_channel_estimation.c:86:11: warning: unused variable ‘ul_ch_estimates’ [-Wunused-variable]
   86 |   c16_t **ul_ch_estimates = (c16_t **)pusch_vars->ul_ch_estimates;
      |           ^~~~~~~~~~~~~~~
/home/bricer/Developer/robert/openairinterface5g/openair1/PHY/NR_ESTIMATION/nr_ul_channel_estimation.c:79:13: warning: unused variable ‘chest_freq’ [-Wunused-variable]
   79 |   const int chest_freq = gNB->chest_freq;
      |             ^~~~~~~~~~
[100%] Linking C static library libPHY_NR.a
WARNING: 3 warnings. See /home/bricer/Developer/robert/openairinterface5g/cmake_targets/log/all.txt
dlsim ulsim ldpctest polartest smallblocktest nr_pbchsim nr_dlschsim nr_ulschsim nr_dlsim nr_ulsim nr_pucchsim nr_prachsim nr_psbchsim params_libconfig coding rfsimulator dfts compiled
BUILD SHOULD BE SUCCESSFUL
```

```
sudo cmake_targets/ran_build/build/nr_ulsim -C 4 -m 25 -s 24 -z 1 -n 100 -P -q 1 -R 273 -r 273
```
> Returns
```powershell
[sudo] password for bricer: 
CMDLINE: "cmake_targets/ran_build/build/nr_ulsim" "-C" "4" "-m" "25" "-s" "24" "-z" "1" "-n" "100" "-P" "-q" "1" "-R" "273" "-r" "273" 
[CONFIG] get parameters from cmdline [CONFIG] debug flags: 0x00400000
Initializing random number generator, seed 2957486406195844388
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
create a thread for core -1
create a thread for core -1
create a thread for core -1
DL frequency 3649140000: band 48, UL frequency 3649140000
[PHY]   Init: N_RB_DL 273, first_carrier_offset 2458, nb_prefix_samples 288,nb_prefix_samples0 352, ofdm_symbol_size 4096
[CONFIG] loader: 2/2 parameters successfully set 
[CONFIG] loader.dfts: 1/2 parameters successfully set 
shlib_path libdfts.so
[LOADER] library libdfts.so successfully loaded
[CONFIG] loader.ldpc: 1/2 parameters successfully set 
shlib_path libldpc.so
[LOADER] library libldpc.so successfully loaded
AWGN: ricean_factor 0.000000
[CONFIG] loader.dfts: 1/2 parameters successfully set 
shlib_path libdfts.so
[LOADER] library libdfts.so has been loaded previously, reloading function pointers
[LOADER] library libdfts.so successfully loaded
num dmrs sym 1
[ULSIM]: length_dmrs: 1, l_prime_mask: 1	number_dmrs_symbols: 1, mapping_type: 1 add_pos: 0 
[ULSIM]: CDM groups: 1, dmrs_config_type: 0, num_rbs: 273, nb_symb_sch: 12
[ULSIM]: MCS: 25, mod order: 8, code_rate: 8850

[ULSIM]: VALUE OF G: 301392, TBS: 262376
*****************************************
SNR 24.000000: n_errors (0/100,0/0,0/0,0/0) (negative CRC), false_positive 100/100, errors_scrambling (30139200/30139200,0/0,0/0,0/0)

SNR 24.000000: Channel BLER (0.000000e+00,-nan,-nan,-nan Channel BER (1.000000e+00,-nan,-nan,-nan) Avg round 1.00, Eff Rate 262376.0000 bits/slot, Eff Throughput 100.00, TBS 262376 bits/slot
DMRS-PUSCH delay estimation: min 0, max 0, average 0.000000
*****************************************

gNB RX
Total PHY proc rx                           971.19 us (100 trials)
 Statistics std=54.09, median=0.00, q1=0.00, q3=0.00 µs (on 0 trials)
|__ RX PUSCH time                          186.13 us (100 trials)
    |__ ULSCH channel estimation time        7.08 us (100 trials)
    |__ RX PUSCH Initialization time        42.08 us (100 trials)
    |__ RX PUSCH Symbol Processing time    136.35 us (100 trials)
|__ ULSCH total decoding time              784.71 us (100 trials)

UE TX
|__ ULSCH total encoding time              331.01 us (100 trials)
    |__ ULSCH segmentation time             20.12 us (100 trials)
    |__ ULSCH LDPC encoder time              0.00 us (  1 trials)
    |__ ULSCH rate-matching time             0.71 us (3200 trials)
    |__ ULSCH interleaving time              3.00 us (3200 trials)
|__ RX SRS time                              0.00 us (  0 trials)
    |__ Generate SRS sequence time           0.00 us (  0 trials)
    |__ Get SRS signal time                  0.00 us (  0 trials)
    |__ SRS channel estimation time          0.00 us (  0 trials)
    |__ SRS timing advance estimation time   0.00 us (  0 trials)
    |__ SRS report TLV build time            0.00 us (  0 trials)
        |__ SRS beam report build time       0.00 us (  0 trials)
        |__ SRS IQ matrix build time         0.00 us (  0 trials)

*************
PUSCH test OK
*************

Num RB:	273
Num symbols:	12
MCS:	25
DMRS config type:	0
DMRS add pos:	0
PUSCH mapping type:	1
DMRS length:	1
DMRS CDM gr w/o data:	1
```

# References

- [ ] [Slides from FOSDEM SDR Devroom part 1 (slides)](https://archive.fosdem.org/2017/schedule/event/oai/attachments/slides/1760/export/events/attachments/oai/slides/1760/oai_L1_L2_procedures_FOSDEM.pdf)
