


```c
#include <stdio.h>
#include <inttypes.h>

typedef struct {
    int est_delay;
} DelayStruct;

int main() {
    int nb_antennas_rx = 4;
    DelayStruct delay[4] = { {1}, {2}, {3}, {4} };
    uint64_t noises_amp2[4] = { 10000000000ULL, 20000000000ULL, 30000000000ULL, 40000000000ULL };

    printf("\n Exit Pool - Starts \n");

    for (int aarx = 0; aarx < nb_antennas_rx; aarx++) {
        printf("Array # = %i\t Estimated delay = %i\t Noise Amp2 = %" PRIu64 "\t\n", aarx, delay[aarx].est_delay, noises_amp2[aarx]);
    }

    printf("\n Exit Pool - Ends \n");

    return 0;
}
```

