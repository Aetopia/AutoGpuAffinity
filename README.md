## AutoGpuAffinity

<img src="./img/exampleoutput.png" width="1000"> 

Automatic GPU affinity benchmarking with [liblava](https://github.com/liblava/liblava)

Contact: https://twitter.com/amitxv

I am not responsible for damage caused to computer. There is a risk of your GPU driver not responding after restarting it during the tests

## Usage

- Windows ADK must be installed for DPC/ISR logging with xperf (this is entirely optional)

    - [ADK for Windows 8.1+](https://docs.microsoft.com/en-us/windows-hardware/get-started/adk-install)
    
    - [ADK for Windows 7](http://download.microsoft.com/download/A/6/A/A6AC035D-DA3F-4F0C-ADA4-37C8E5D34E3D/setup/WinSDKPerformanceToolKit_amd64/wpt_x64.msi)

- Maintain overclock settings with MSI Afterburner throughout the benchmark

    - Save the desired settings to a profile (e.g profile 1)

    - Configure the path along with the profile to load in **config.txt**
    
- Download & extract the latest release from the [releases tab](https://github.com/amitxv/AutoGpuAffinity/releases)

- Run **start.bat** & press enter when ready

- After the tool has benchmarked each core, the GPU affinity will be reset to the Windows default & a table will be displayed with the results. The xperf report is located in the session directory

- Run the tool two or three times. If the same core is consistently performant & no 0.005% Lows values are absurdly low compared to other results, then your results are reproducible & your testing environment is consistent

