

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
