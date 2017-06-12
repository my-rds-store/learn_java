########
安装java
########


.. image:: ./images/java.jpg 
       :scale: 100%
       :alt: alternate text
       :align: center

下载
====

http://www.oracle.com/technetwork/java/javase/overview/index.html


.. code:: sh

    $ sudo tar xzvf jdk-8u131-linux-x64.tar.gz -C /opt/
    $ cd /opt/jdk1.8.0_131


编辑 **$HOME/.bash_aliases** 

.. code:: sh

    # config java
    export JAVA_HOME=/opt/jdk1.8.0_131  
    export JRE_HOME=${JAVA_HOME}/jre  
    export CLASSPATH=.:${JAVA_HOME}/lib:${JRE_HOME}/lib  
    export PATH=${JAVA_HOME}/bin:$PATH

.. code:: sh

    $ java -version

