# Read Me

The library provides a Python class wrapper for FLIR Systems's Blackfly USB3 Camera.

By Chris Arcadia 

Created on 2021/01/01. 

Intended for use with the FLIR's Blackfly S USB3:
*  Model: BFS-U3-04S2C-CS
*  Resolution: 0.4 MP
*  Speed: 522 FPS
*  Sensor Model: Sony IMX287
*  Sensor Type: CMOS
*  Chroma: Color
*  Interface: USB 3
*  Link: https://www.flir.com/products/blackfly-s-usb3/

## Software Requirements
* FLIR [Spinnaker](https://www.flir.com/products/spinnaker-sdk/) driver 
  * The pywheel for Spinnaker can be found [here](https://meta.box.lenovo.com/v/link/view/a1995795ffba47dbbe45771477319cc3). The `spinnaker_python-2.2.0.48-cp36-cp36m-win_amd64.zip` archive from [FLIR Support/Spinnaker/Windows/python](https://meta.box.lenovo.com/v/link/view/a1995795ffba47dbbe45771477319cc3) was used in this repository.
  * Install Spinnaker wheel by running: `pip install spinnaker_python-2.2.0.48-cp36-cp36m-win_amd64.whl` after going through the driver read-me file and making the necessarying package installations.
  * Install the Spinnaker app for windows (for this repository we installed `SpinnakerSDK_FULL_2.2.0.48_x64.exe` from [here](https://meta.box.lenovo.com/v/link/view/a1995795ffba47dbbe45771477319cc3))
  * Further documentation can be found [here](http://softwareservices.flir.com/Spinnaker/latest/index.html) 
* [Anaconda 3](https://www.anaconda.com/) (`Anaconda3-4.4.0-Windows-x86.exe` from the [installer archive](https://repo.anaconda.com/archive/) was used for development)
* for Python to access the driver, use the [ctypes](https://docs.python.org/3/library/ctypes.html) package


## Hardware Requirements

* FLIR Blackfly USB 3 camera.
  * DeviceDisplayName: Point Grey Research Blackfly S BFS-U3-51S5C
  * DeviceModelName: Blackfly S BFS-U3-51S5C
  * DeviceType: USB3Vision
  * DeviceVendorName: Point Grey Research
  * DeviceCurrentSpeed: SuperSpeed
  * DeviceVersion: 1605.1.3.0
  * DeviceDriverVersion: PGRUSBCam3.sys : 2.7.3.249
* CPU with USB 3 and enough RAM for the Python program to run.

