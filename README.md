# PiLapseRails
raspberry timelapse rails contriller for use with a smartphone
  
## Getting Started

instructions 

### Prerequisities

What things you need to install the software and how to install them

```
Give examples
```

### Installing

-Get a [rasbian](https://www.raspberrypi.org/help/quick-start-guide/) installed on your PI
-connect to wifi/ethernet
-open up terminal (the black monitor icon) and enter  the following commands:
```
sudo apt-get update //(in case its a fresh rasbian installation)

sudo apt-get install nodejs npm //installs [nodejs](https://nodejs.org/en/)
sudo npm install -g express
git clone git://github.com/equilerex/quick2wire-gpio-admin-permission-fix // provides permission to use pins
cd quick2wire-gpio-admin-permission-fix/
make
sudo make install
sudo adduser $USER gpio
cd ..
git clone git://github.com/equilerex/PiLapseRails // our actual project
cd PiLapseRails/
npm install
cd ..
sudo nano etc/rc.local
use arrows to move to the end of the file and type:
su pi -c 'node /home/pi/PiLapseRails/bin/www.js < /dev/null &'
ctrl + o
enter to confirm
make a tethered hotspot (portable wifi got-spot) on the phone you'll be using
on pi, connect to that hotspot. if you are at home and used the wifi for setting everything up, you might want to remove that wifi so the pi would always connect to the phone automatically
reboot

ifconfig

```




Stay what the step will be

```
Give the example
```

And repeat

```
until finished
```

End with an example of getting some data out of the system or using it for a little demo

## Running the tests

Explain how to run the automated tests for this system

### Break down into end to end tests

Explain what these tests test and why

```
Give an example
```

### And coding style tests

Explain what these tests test and why

```
Give an example
```

## Deployment

Add additional notes about how to deploy this on a live system

## Built With

* Dropwizard - Bla bla bla
* Maven - Maybe
* Atom - ergaerga

## Contributing

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags). 

## Authors

* **Billie Thompson** - *Initial work* - [PurpleBooth](https://github.com/PurpleBooth)

See also the list of [contributors](https://github.com/your/project/contributors) who participated in this project.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Hat tip to anyone who's code was used
* Inspiration
* etc