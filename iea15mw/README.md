# debug_BD_DT
Model: IEA 15MW, no gravity, no aero, no cone tilt overhang, curved blade
* Test0: BeamDyn driver, azimuth 0 deg, hub of 1m. It runs with DT = 0.01s
* Test1: BeamDyn driver, azimuth 90 deg, hub of 1m. It does NOT run with DT = 0.01s (down to 0.0001s did not work)
* Test2: BeamDyn driver, azimuth 90 deg, hub of 0m. It runs with DT = 0.01s. Fails after 13 seconds.
* Test3: OpenFAST driver calling BD, hub of 0m. It runs with DT = 0.0006s. Largest value is 0.00065s (manually checked).