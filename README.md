# bebop_autonomy

[ROS](http://ros.org) driver for [Parrot Bebop](http://www.parrot.com/ca/products/bebop-drone/) drone (quadrocopter).

* Documentation: http://bebop-autonomy.readthedocs.io/
* ROS wiki page: http://wiki.ros.org/bebop_autonomy
* Support: [ROS Q&A (tag: bebop_autonomy)](http://answers.ros.org/questions/scope:all/sort:activity-desc/tags:bebop_autonomy/page:1/)
* Code API: http://docs.ros.org/indigo/api/bebop_autonomy/html

## Development Team

* Author: [Mani Monajjemi](http://mani.im) ([Autonomy Lab](http://autonomylab.org), [Simon Fraser University](http://www.sfu.ca)) + [other contributers](http://bebop-autonomy.readthedocs.io/en/latest/contribute.html#list-of-contributers)
* Maintainers:
    * [Sepehr MohaimenianPour](http://sepehr.im/) ([Autonomy Lab](http://autonomylab.org), [Simon Fraser University](http://www.sfu.ca))
    * Thomas Bamford ([Dynamic Systems Lab](http://www.dynsyslab.org), [University of Toronto](https://www.utoronto.ca/))
    * [Tobias Naegeli](https://ait.ethz.ch/people/naegelit/) ([Advanced Interactive Technologies Lab](http://www.ait.ethz.ch/), [ETH Zürich](http://www.ethz.ch/))

## Build Status

[![Build Status (ROS I,J,K) - TravisCI](https://travis-ci.org/AutonomyLab/bebop_autonomy.svg?branch=indigo-devel)](https://travis-ci.org/AutonomyLab/bebop_autonomy) [![Build Status (ROS I,J) - Semaphore](https://semaphoreci.com/api/v1/projects/11786233-d505-4d79-b27c-80c2742243a4/537552/badge.svg)](https://semaphoreci.com/mani_monaj/bebop_autonomy)

Built against [parrot_arsdk](https://github.com/AutonomyLab/parrot_arsdk) 3.14.0p1

## Melodic build

In order to build `bebop_autonomy` on melodic, first install `parrot_arsdk`.
It is available as binary package and use following command: 
```
sudo apt-get install ros-melodic-parrot-ardsk`
```

After that it's neccessary to add built libraries to the `LD_LIBRARY_PATH` as follows: 
```
echo LD_LIBRARY_PATH=/usr/local/lib/parrot_arsdk/:$LD_LIBRARY_PATH >> ~/.bashrc
source ~/.bashrc	
```

After you've added `parrot_arsdk` libraries to LD_LIBRARY_PATH you need to build 
`bebop_autonomy` with `catkin_make` as follows: 

```
cd <path_to_catkin_ws>
catkin_make
source devel/setup.bash
```


