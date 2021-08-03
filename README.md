

# mmwave-energy ns-3 module #

This is an [ns-3](https://www.nsnam.org "ns-3 Website") mmwave-energy module for analyzing and exploring the power consumption behavior of 5G communication protocols under NR technology. The module developed includes a complete Radio Resource Control(RRC) state machine for 5G NR recommended by 3GPP specification [38.840]. [Ns-3 mmwave](https://github.com/nyuwireless-unipd/ns3-mmwave "mmWave ns-3 module") is used as a base, on top of which we will add our module as plug-in.


### Brand new installation of ns3-mmwave repository

To download a working copy of the ns3-mmwave repository with the latest changes,
you can do the following:

```
$ git clone https://github.com/nyuwireless-unipd/ns3-mmwave.git
$ cd ns3-mmwave
```

### Test the installation
To test the installation, after following one of the previous point, you can do
a simple configuration and compile test (more options for that later):

```
$ ./waf configure --enable-examples --enable-tests
$ ./waf
```

A success for both previous commands indicates an overall success.

### Brand new installation of the mmwave-energy module

As a precondition to the following steps, you must have a working local git
repository of ns3-mmwave. If that is the case, then, your local git repo is ready
to include our mmwave module

```
$ cd src
$ git clone https://github.com/arghasen10/mmwave-energy.git
$ cd ..
```

Please note that the src/mmwave-energy directory will be listed as "Untracked files" every
time you do a `git status` command. Ignore it, as the directory lives as an
independent module. As a result, we have now two parallel repository, but one
lives inside the other.

### Test the mmwave-energy installation

Let's configure the project:

```
$ ./waf configure --enable-examples --enable-tests
```

If the mmwave-energy module is recognized correctly, you should see "mmwave-energy" in the list of
built modules. If that is not the case, then most probably the previous
point failed. Otherwise, you could compile it:

```
$ ./waf
```

## Papers
 - IEEE INFOCOM, Poster, 2021 - Authors: [Argha Sen](https://arghasen10.github.io/ "My Webpage"), Abhijit Mondal, Basabdatta Palit, Jay Jayatheerthan, Krishna Paul, Sandip Chakraborty [An ns3-based Energy Module of 5G NR User Equipments for Millimeter Wave Networks](https://ieeexplore.ieee.org/document/9484493 "IEEE Publication")

## Future work
 - Hardware & network throughput dependency on energy consumption.
 - cDRX implementation for Efficient energy consumption.
## Authors ##

 - Argha Sen
 - Abhijit Mondal
 - Basabdatta Palit
 - Sandip Chakraborty 

## License ##

This software is licensed under the terms of the GNU GPLv2, as like as ns-3.
See the LICENSE file for more details.
