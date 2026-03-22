### 🚀 Quick Start with YaarScript

Save this in a `.yaar` file and run it with the compiler:

```rust
// 2. Karo-Jabtak Loop (Diagnostics)
bolo("[2] Running Sensor Calibration:\n");
number attempt = 1;
faisla sensor_ready = galat;

karo {
    bolo("Probe #", attempt, ":\t");
    agar (attempt < 10) {
        bolo("Warming up...\n");
    } warna {
        bolo("Calibration Complete!\n");
        sensor_ready = sahi;
    }
    attempt = attempt + 1;
} jabtak (!sensor_ready);
