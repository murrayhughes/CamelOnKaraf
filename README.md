# Camel, Karaf and freinds

Tired of waiting for servicemix to upgrade its dependencies...
Here is the current Karaf version with the current Camel, CXF, ActiveMQ and Hawtio management console on top.

This lacks servicemix's features, and servicemix's testing.
But, if all you want is Camel running in Karaf, and you will test your app, then this may suit.

Install:
0) Get experienced at using Servicemix.
1) Install Karaf 4.1.5
2) copy jetty.xml in the karaf/etc folder. (its just a copy of the servicemix one)
3) review features-deploy-camel.xml adding any features you need.
4) copy features-deploy-camel.xml into the deploy folder
5) copy example route route-amq1.xml to the deploy folder - that will activate activemq, camel.
6) Start karaf and watch the logs...
7) browse to http://localhost:8181/hawtio log in with karaf/karaf
