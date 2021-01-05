VelodyneCapture
===============

VelodyneCapture is the general capture class to retrieve the laser data from Velodyne sensors using Boost.Asio and PCAP.  
VelodyneCapture will be able to retrieve lasers infomation about azimuth, vertical and distance that capture at one rotation or a single data packet.  
This class supports direct capture form Velodyne sensors, or capture from PCAP files.  
( This class only supports VLP-16 and HDL-32E sensor, it does not support Dual Return mode. )  


Environment
-----------
If direct capture from sensors is desired, VelodyneCapture requires Boost.Asio and its dependent libraries ( Boost.System, Boost.Date_Time, Boost.Regex ).  
Please define <code>HAVE_BOOST</code> in preprocessor.  
* Boost.Asio  
If capture from PCAP files is instead desired, VelodyneCapture requires PCAP.  
Please define <code>HAVE_PCAP</code> in preprocessor.  
* libpcap ( or WinPCAP )  


Sample
------
This repository has two sample programs.  

* velodyne_viewer  
  This sample program displays data on a point cloud viewer.  
  This sample program depends on the above libraries ( Boost.Asio or libpcap ( or WinPCAP ) ) of VelodyneCapture class.  


To do
* UKF
