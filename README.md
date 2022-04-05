<div id="top"></div>
<!-- PROJECT SHIELDS -->
<!-- END OF PROJECT SHIELDS -->

<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="#">
    <img src="/images/logo.png" alt="Logo" height="200">
  </a>

<h3 align="center">Epitaph IPS</h3>

  <p align="center">
    <i>Library with utilities to calculate a users position written in Dart</i>
    <br /><a href="#">Report Bug</a>
    ·
    <a href="#">Request Feature</a>
  </p>
</div>

<!-- ABOUT THE PROJECT -->
## About The Project

Epitaph has a wide array of utilities to position your user in a building. The project is intended to be used to only calculate the position on the user's device. 
It has been written in Dart using the Flutter framework. Bluetooth Low Energy (BLE) beacons are used to make the calculations possible.
Received Signal Strength Indication (RSSI) values are used to calculate the user’s location in the real world. 
<p align="right">(<a href="#top">back to top</a>)</p>



### Built With

This library has been build with:
 - [Flutter](https://flutter.dev/)


<p align="right">(<a href="#top">back to top</a>)</p>

## Installation

<i>Will be updated</i>

<p align="right">(<a href="#top">back to top</a>)</p>

## Usage

<i>In Progress</i>

### Tracking
The tracking system consists of multiple modules that can theoretically be used individually as well.

#### Module descriptions
- **Calculator** - module for calculating a raw position through the use of read values, i.e. RSSI-values from BLE beacons
- **Filter** - module for smoothening out raw positions. This can be particularly useful when values tend to be noisy
- **Tracker** - module that uses Calculator and Filter to contininuosly track the user's position
- **Mapper** (inherits from Tracker) - module for tracking a user's position on a map (with correlating graph, nodes and edges)

#### Calculator
- consists of `Coordinate calculate(List<Beacon>)`
- reads certain values from said list and calculates a position using those values

#### Filter
- consists of `Coordinate filter(Coordinate)`, `void configFilter(Coordinate)`, `void reset()`
- an implemented filter should continuously take in a coordinate, process it and save the result for upcoming processing
- 

#### Tracker

#### Mapper

## Documentation
<i>Will be updated</i>

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please open an issue with the tag "enhancement", fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Open an issue with the tag "enhancement"
2. Fork the Project
3. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
4. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
5. Push to the Branch (`git push origin feature/AmazingFeature`)
6. Open a Pull Request

The Flutter Team has a great guide [here](https://docs.flutter.dev/get-started/install) how to set up everything needed.

We also would suggest looking into the Flutter Team's style guide [here](https://github.com/flutter/flutter/wiki/Style-guide-for-Flutter-repo)

More about this in the [CODE_OF_CONDUCT](/CODE_OF_CONDUCT.md) file.

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- ROADMAP -->
## Roadmap


See the [open issues](#) for a full list of proposed features, known issues and out latest Roadmap.

<p align="right">(<a href="#top">back to top</a>)</p>


<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE` file for more information.

<p align="right">(<a href="#top">back to top</a>)</p>


<!-- CONTACT -->
## Contact

it@m - opensource@muenchendigital.io

[join our slack channel](https://join.slack.com/t/epitaph-ips/shared_invite/zt-164oqyxvl-pNIGa9n6jA1fJZmk1h6zeg)

<p align="right">(<a href="#top">back to top</a>)</p>


<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
