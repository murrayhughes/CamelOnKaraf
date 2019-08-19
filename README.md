# Camel On Karaf Additive

Here is the current Karaf version with the current versions of Camel, CXF, ActiveMQ and Hawtio management console on top.
Makes creating a camel route as easy as editing an xml file in the deploy folder. 
Start with Karaf & add Camel etc.  Karaf will download them from the net.  Adjust the dependency versions by editing features-deploy-camel.xml.

This lacks all servicemix's features, and lacks servicemix's testing.
But, if all you want is Camel running in Karaf, and you will test your app, then this may suit.


0) Install java 11.
1) Download & unzip Karaf 4.2.6 (into a top-level windows folder, with no spaces in its name)
2) Optionally copy jetty.xml in the karaf/etc folder. (its just a copy of the servicemix one)
3) review features-deploy-camel.xml adding any extra features you need.
4) copy features-deploy-camel.xml into the deploy folder
5) copy example route route-amq1.xml to the deploy folder - that will activate activemq, camel.
6) run karaf.bat & wait for karaf to download & start camel.
7) browse to http://localhost:8181/hawtio log in with karaf/karaf
8) Write your camel route by editing example route route-amq1.xml

