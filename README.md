OpenShift ElasticSearch Cartridge
=================================
Downloadable ElasticSearch cartridge for OpenShift.

To create your scalable ElasticSearch app, run:

    rhc app create <your app name> https://raw.githubusercontent.com/chifeo/OpenShift-ElasticSearch-1.3.2-Catridge/master/openshift-elasticsearch-cartridge -s

**NOTE:** your app currently must be a scalable app or this cartridge will not run.


Adding additional cluster nodes
===============================
To add more nodes to the cluster, simply add more gears:

    rhc cartridge scale -a <your app name> elasticsearch <number of total gears you want>


Plugins
=======
To install ElasticSearch plugins, edit the `plugins.txt` file, commit, and push your changes.

See more
=======
https://github.com/ncdc/openshift-elasticsearch-cartridge

License
=======
This project is licensed under the [Apache License 2.0](http://www.apache.org/licenses/LICENSE-2.0.html).
