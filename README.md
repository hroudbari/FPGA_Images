# FPGA_Images
FPGA Images (from my synthesis flow)

To run Checksum Calculation Application, first follow instructions on server side, then go to client instructions.

On Server:
1. git clone https://github.com/hroudbari/FPGA_Images.git
2. Program golden_checksum.mcs on the FPGA (user image)
3. Power cycle the server.
4. Load FPGA image from user image
5. Run "python binary_server.py"
6. run "tcpdump -i eth0 -w traffic.pcap" in separate terminal to capture network traffic 
7. Run client instructions.
8. Do a ctrl+c on the server to stop pcap capture.
9. Email "traffic.pcap" to hseyedro3@gatech.edu


On Client:
1. git clone https://github.com/hroudbari/FPGA_Images.git
2. Run "python binary_client.py" 5 times.