# Case study — Building the measurement chain first

**Problem:** offboard software needs measurements whose units, timing, calibration and failures are understood.

**Approach:** isolate a USB bench, emit raw CSV with device/session/sequence/uptime and health flags, check structure on the host, then qualify the complete chain before vehicle use.

**Implementation evidence:** recovered 19 August PlatformIO and Arduino firmware packages, a bare-ESP32 USB sketch, provisional pin map, CSV validator and physical run sheet. Existing founder records support upload/serial checks; they do not establish integrated sensor logging.

**Result boundary:** consolidation can validate host-generated files and source preservation. There is no genuine integrated bench session, calibrated accuracy result, vehicle-interface test or direct OctaneOS import result.

**Decision learned:** `voltage_v` on an isolated 3.3 V ADC bench is not automatically a battery-voltage measurement. The currently recovered firmware/importer contracts differ in names, schema marker, identity and time requirements.

**Next:** actual module identification, multimeter references, repeated 10 Hz bench evidence, SD continuity/power-loss checks and a declared software handoff contract.
