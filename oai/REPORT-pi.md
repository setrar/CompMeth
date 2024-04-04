


```
./build_oai --phy_simulators
```
> Returns
```powershell
Will compile dlsim, ulsim, ...
OPENAIR_DIR    = /home/ubuntu/Developer/gitlab.eurecom.fr/openairinterface5g
Running "cmake ../../.."
-- The C compiler identification is GNU 13.2.0
-- The CXX compiler identification is GNU 13.2.0
-- Detecting C compiler ABI info
-- Detecting C compiler ABI info - done
-- Check for working C compiler: /usr/bin/cc - skipped
-- Detecting C compile features
-- Detecting C compile features - done
-- Detecting CXX compiler ABI info
-- Detecting CXX compiler ABI info - done
-- Check for working CXX compiler: /usr/bin/c++ - skipped
-- Detecting CXX compile features
-- Detecting CXX compile features - done
-- Ccache not found. Consider installing it for faster compilation. Command: sudo apt/dnf install ccache
-- Found PkgConfig: /usr/bin/pkg-config (found version "1.8.1") 
-- Check if /opt/asn1c/bin/asn1c supports -gen-APER
-- Check if /opt/asn1c/bin/asn1c supports -no-gen-UPER
-- Check if /opt/asn1c/bin/asn1c supports -no-gen-JER
-- Check if /opt/asn1c/bin/asn1c supports -no-gen-BER
-- Check if /opt/asn1c/bin/asn1c supports -no-gen-OER
-- CMAKE_BUILD_TYPE is RelWithDebInfo
-- CPU architecture is aarch64
-- Found Git: /usr/bin/git (found version "2.40.1") 
-- Selected E2AP_VERSION: E2AP_V2
-- Selected KPM Version: KPM_V2_03
-- Checking for module 'libconfig'
--   Found libconfig, version 1.5
-- Checking for module 'openssl'
--   Found openssl, version 3.0.10
-- Checking for module 'blas'
--   Found blas, version 3.10.3
-- Checking for module 'lapacke'
--   Found lapacke, version 3.11.0
-- Checking for module 'cblas'
--   Package 'cblas', required by 'virtual:world', not found
-- No Support for Aerial
-- No Doxygen documentation requested
-- Configuring done (2.7s)
-- Generating done (3.6s)
-- Build files have been written to: /home/ubuntu/Developer/gitlab.eurecom.fr/openairinterface5g/cmake_targets/ran_build/build
cd /home/ubuntu/Developer/gitlab.eurecom.fr/openairinterface5g/cmake_targets/ran_build/build
Running "cmake --build .  --target dlsim ulsim ldpctest polartest smallblocktest nr_pbchsim nr_dlschsim nr_ulschsim nr_dlsim nr_ulsim nr_pucchsim nr_prachsim params_libconfig coding rfsimulator dfts -- -j4" 
Log file for compilation is being written to: /home/ubuntu/Developer/gitlab.eurecom.fr/openairinterface5g/cmake_targets/log/all.txt
/usr/include/simde/arm/neon/get_lane.h:279:5: error: incompatible type for argument 1 of ‘vget_lane_f16’
  279 |     SIMDE_CONSTIFY_8_(vget_lane_f16, r, (HEDLEY_UNREACHABLE(), SIMDE_FLOAT16_VALUE(0.0)), lane, v);
      |     ^~~~~~~~~~~~~~~~~
      |     |
--
/usr/include/simde/arm/neon/get_lane.h:279:5: error: incompatible type for argument 1 of ‘vget_lane_f16’
  279 |     SIMDE_CONSTIFY_8_(vget_lane_f16, r, (HEDLEY_UNREACHABLE(), SIMDE_FLOAT16_VALUE(0.0)), lane, v);
      |     ^~~~~~~~~~~~~~~~~
      |     |
--
/usr/include/simde/arm/neon/get_lane.h:279:5: error: incompatible type for argument 1 of ‘vget_lane_f16’
  279 |     SIMDE_CONSTIFY_8_(vget_lane_f16, r, (HEDLEY_UNREACHABLE(), SIMDE_FLOAT16_VALUE(0.0)), lane, v);
      |     ^~~~~~~~~~~~~~~~~
      |     |
--
/usr/include/simde/arm/neon/get_lane.h:279:5: error: incompatible type for argument 1 of ‘vget_lane_f16’
  279 |     SIMDE_CONSTIFY_8_(vget_lane_f16, r, (HEDLEY_UNREACHABLE(), SIMDE_FLOAT16_VALUE(0.0)), lane, v);
      |     ^~~~~~~~~~~~~~~~~
      |     |
--
/usr/include/simde/arm/neon/get_lane.h:279:5: error: incompatible type for argument 1 of ‘vget_lane_f16’
  279 |     SIMDE_CONSTIFY_8_(vget_lane_f16, r, (HEDLEY_UNREACHABLE(), SIMDE_FLOAT16_VALUE(0.0)), lane, v);
      |     ^~~~~~~~~~~~~~~~~
      |     |
--
/usr/include/simde/arm/neon/get_lane.h:279:5: error: incompatible type for argument 1 of ‘vget_lane_f16’
  279 |     SIMDE_CONSTIFY_8_(vget_lane_f16, r, (HEDLEY_UNREACHABLE(), SIMDE_FLOAT16_VALUE(0.0)), lane, v);
      |     ^~~~~~~~~~~~~~~~~
      |     |
--
/usr/include/simde/arm/neon/get_lane.h:279:5: error: incompatible type for argument 1 of ‘vget_lane_f16’
  279 |     SIMDE_CONSTIFY_8_(vget_lane_f16, r, (HEDLEY_UNREACHABLE(), SIMDE_FLOAT16_VALUE(0.0)), lane, v);
      |     ^~~~~~~~~~~~~~~~~
      |     |
--
/usr/include/simde/arm/neon/get_lane.h:279:5: error: incompatible type for argument 1 of ‘vget_lane_f16’
  279 |     SIMDE_CONSTIFY_8_(vget_lane_f16, r, (HEDLEY_UNREACHABLE(), SIMDE_FLOAT16_VALUE(0.0)), lane, v);
      |     ^~~~~~~~~~~~~~~~~
      |     |
--
/usr/include/simde/arm/neon/get_lane.h:279:5: error: incompatible type for argument 1 of ‘vget_lane_f16’
  279 |     SIMDE_CONSTIFY_8_(vget_lane_f16, r, (HEDLEY_UNREACHABLE(), SIMDE_FLOAT16_VALUE(0.0)), lane, v);
      |     ^~~~~~~~~~~~~~~~~
      |     |
--
/usr/include/simde/arm/neon/get_lane.h:279:5: error: incompatible type for argument 1 of ‘vget_lane_f16’
  279 |     SIMDE_CONSTIFY_8_(vget_lane_f16, r, (HEDLEY_UNREACHABLE(), SIMDE_FLOAT16_VALUE(0.0)), lane, v);
      |     ^~~~~~~~~~~~~~~~~
      |     |
--
/usr/include/simde/arm/neon/get_lane.h:279:5: error: incompatible type for argument 1 of ‘vget_lane_f16’
  279 |     SIMDE_CONSTIFY_8_(vget_lane_f16, r, (HEDLEY_UNREACHABLE(), SIMDE_FLOAT16_VALUE(0.0)), lane, v);
      |     ^~~~~~~~~~~~~~~~~
      |     |
--
/usr/include/simde/arm/neon/get_lane.h:279:5: error: incompatible type for argument 1 of ‘vget_lane_f16’
  279 |     SIMDE_CONSTIFY_8_(vget_lane_f16, r, (HEDLEY_UNREACHABLE(), SIMDE_FLOAT16_VALUE(0.0)), lane, v);
      |     ^~~~~~~~~~~~~~~~~
      |     |
--
/usr/include/simde/arm/neon/get_lane.h:279:5: error: incompatible type for argument 1 of ‘vget_lane_f16’
  279 |     SIMDE_CONSTIFY_8_(vget_lane_f16, r, (HEDLEY_UNREACHABLE(), SIMDE_FLOAT16_VALUE(0.0)), lane, v);
      |     ^~~~~~~~~~~~~~~~~
      |     |
--
/usr/include/simde/arm/neon/get_lane.h:279:5: error: incompatible type for argument 1 of ‘vget_lane_f16’
  279 |     SIMDE_CONSTIFY_8_(vget_lane_f16, r, (HEDLEY_UNREACHABLE(), SIMDE_FLOAT16_VALUE(0.0)), lane, v);
      |     ^~~~~~~~~~~~~~~~~
      |     |
--
/usr/include/simde/arm/neon/get_lane.h:279:5: error: incompatible type for argument 1 of ‘vget_lane_f16’
  279 |     SIMDE_CONSTIFY_8_(vget_lane_f16, r, (HEDLEY_UNREACHABLE(), SIMDE_FLOAT16_VALUE(0.0)), lane, v);
      |     ^~~~~~~~~~~~~~~~~
      |     |
--
/usr/include/simde/arm/neon/get_lane.h:279:5: error: incompatible type for argument 1 of ‘vget_lane_f16’
  279 |     SIMDE_CONSTIFY_8_(vget_lane_f16, r, (HEDLEY_UNREACHABLE(), SIMDE_FLOAT16_VALUE(0.0)), lane, v);
      |     ^~~~~~~~~~~~~~~~~
      |     |
--
/usr/include/simde/arm/neon/sqrt.h:40:26: error: ‘b’ undeclared (first use in this function)
   40 |     return vsqrth_f16(a, b);
      |                          ^
/usr/include/simde/arm/neon/sqrt.h:40:26: note: each undeclared identifier is reported only once for each function it appears in
/usr/include/simde/arm/neon/sqrt.h:40:12: error: too many arguments to function ‘vsqrth_f16’
   40 |     return vsqrth_f16(a, b);
      |            ^~~~~~~~~~
In file included from /usr/lib/gcc/aarch64-linux-gnu/13/include/arm_neon.h:25590:
--
/usr/include/simde/arm/neon/sqrt.h:40:26: error: ‘b’ undeclared (first use in this function)
   40 |     return vsqrth_f16(a, b);
      |                          ^
/usr/include/simde/arm/neon/sqrt.h:40:26: note: each undeclared identifier is reported only once for each function it appears in
/usr/include/simde/arm/neon/sqrt.h:40:12: error: too many arguments to function ‘vsqrth_f16’
   40 |     return vsqrth_f16(a, b);
      |            ^~~~~~~~~~
In file included from /usr/lib/gcc/aarch64-linux-gnu/13/include/arm_neon.h:25590:
--
/home/ubuntu/Developer/gitlab.eurecom.fr/openairinterface5g/openair1/PHY/TOOLS/oai_dfts_neon.c:1540:25: warning: unused variable ‘tw512_128p’ [-Wunused-variable]
 1540 |   simd_q15_t ytmp[128],*tw512_128p=(simd_q15_t*)tw512,*tw512a_128p=(simd_q15_t *)tw512a,*tw512b_128p=(simd_q15_t *)tw512b,*y128=(simd_q15_t *)y,*y128p=(simd_q15_t *)y;
      |                         ^~~~~~~~~~
gmake[3]: *** [CMakeFiles/dfts.dir/build.make:90: CMakeFiles/dfts.dir/openair1/PHY/TOOLS/oai_dfts_neon.c.o] Error 1
WARNING: 1 warnings. See /home/ubuntu/Developer/gitlab.eurecom.fr/openairinterface5g/cmake_targets/log/all.txt
ERROR: 20 error. See /home/ubuntu/Developer/gitlab.eurecom.fr/openairinterface5g/cmake_targets/log/all.txt
compilation of dlsim ulsim ldpctest polartest smallblocktest nr_pbchsim nr_dlschsim nr_ulschsim nr_dlsim nr_ulsim nr_pucchsim nr_prachsim params_libconfig coding rfsimulator dfts failed
build have failed
```
