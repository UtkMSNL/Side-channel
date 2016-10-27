Greetings,

To prevent the low-latency traffic from suffering excessive queueing delay, in this project, we encodes delay-sensitive traffic (referred to as side channel) as different patterns of interference, and deliver them along with the regular WiFi frame transmission (referred to as main channel). We use symbols erasing as the form of interference. To implement this, a new module named "side_channel_mod" is introduced, which decides whether to maintain or to erase the main channel symbol energy according to the content of side channel data. In the receiver side, the main channel suffers little degradation and can be recovered through regular decoding procedure. In addition, side channel information can be detected through comparing symbol energy: symbols being erased exhibit smaller power in the receiver side compared to others.

This project is built upon GNURadio/USRP platform. The project is built upon project IEEE802.11 PHY (https://github.com/bastibl/gr-ieee802-11/).
 
To use this project, please cite the following literatures:

1) Side channel design

@inproceedings{lu2016supporting,
  title={Supporting real-time wireless traffic through a high-throughput side channel},
  author={Lu, Haoyang and Gao, Wei},
  booktitle={Proceedings of the 17th ACM International Symposium on Mobile Ad Hoc Networking and Computing},
  pages={311--320},
  year={2016},
  organization={ACM}
}

2 The PHY implementation is based on (https://github.com/bastibl/gr-ieee802-11/)

@inproceedings{bloessl2013ieee,
  title={An IEEE 802.11 a/g/p OFDM Receiver for GNU Radio},
  author={Bloessl, Bastian and Segata, Michele and Sommer, Christoph and Dressler, Falko},
  booktitle={Proceedings of the second workshop on Software radio implementation forum},
  pages={9--16},
  year={2013},
  organization={ACM}
}

# Installation
For installation of GNURadio and libraries, please refer to (https://github.com/bastibl/gr-ieee802-11/).

# Further information
For details of the project, please refer to the paper 1. If you have any further questions, please contact
Haoyang Lu, (hlu9@utk.edu)
University of Tennessee
