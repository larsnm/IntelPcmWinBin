# Intel PCM Windows Binaries for Testing

Disclaimer: The provided binaries of Intel PCM are soely for testing purpose with the CARLsim Performance Monitor and for non commercial usage. For production scenarios, build Intel PCM from source following the instructions provided by Intel on GitHub https://github.com/intel/pcm/blob/master/doc/WINDOWS_HOWTO.md . As this requires system level skills, you might want to plan for professional support in sponsored project setups. 
 
## Installation 
Copy or clone the repository to the directory C:\Program Files\PCM and add it to the Path variable. This requires administration rights. The Windows MSR driver was signed with the generated test certificate and the password test. Import MSR.cert to "Current User" and when able to pick "Place all ...", browse for "Trusted Root Certification Authorities", see also https://github.com/intel/pcm/blob/master/doc/WINDOWS_HOWTO.md#sign-the-windows-msr-driver .

## Usage 
Open a command prompt as administrator and start  pcm.exe 

For more information see GitHub https://github.com/intel/pcm.

## Development
The header files are located in the directory include. For release builds, the libraries are located in the directory lib, for debugging, in the directory debug.   

## Build information
The binaries were built on the following stack: 
- Microsoft Visual Studio Community 2022, Version 17.14.9
- Windows Driver Kit, Version 10.0.26100.2454

.