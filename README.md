tf_splitter
===========

1. About

    The tf_splitter package contains a ROS node that decomposes the /tf topic into multiple ones according to the number of robots. This package can be used in multi-robot systems to alleviate the network traffic load.

2. Nodes

    2.1 tf_splitter
    
    tf_splitter decomposes the /tf topic into multiple ones according to the number of robots.

    2.1.1 Subscribed Topics

    /tf (tf/tfMessage)
        Transform tree. 

    2.1.2 Published Topics

    /<tf prefix according to the robots> (tf/tfMessage)
        Splitted transform tree.
        
3. Usage

    rosrun tf_splitter tf_splitter

4. Related Documentation

    Please refer to the following paper to retrieve more information on the node:

    @inproceedings{yz14simpar,
    author = {Zhi Yan and Luc Fabresse and Jannik Laval and Noury Bouraqadi},
    title = {Team Size Optimization for Multi-robot Exploration},
    booktitle = {In Proceedings of the 4th International Conference on Simulation, Modeling, and Programming for Autonomous Robots (SIMPAR 2014)},
    pages = {438--449},
    address = {Bergamo, Italy},
    month = {October},
    year = {2014}
    }

5. Support

    Zhi Yan, Luc Fabresse, Jannik Laval, and Noury Bouraqadi
    Ecole des Mines de Douai, 59508 Douai, France
    http://car.mines-douai.fr
