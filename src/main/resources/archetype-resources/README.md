${artifactId}
===========
[![Build Status](https://travis-ci.org/DANS-KNAW/${artifactId}.png?branch=master)](https://travis-ci.org/DANS-KNAW/${artifactId})

<!-- Remove this comment and extend the descriptions below -->


SYNOPSIS
--------

    ${artifactId} (synopsis of command line parameters)
    ${artifactId} (... possibly multiple lines for subcommands)


DESCRIPTION
-----------

${description}


ARGUMENTS
---------

    Options:

       -h, --help      Show help message
       -v, --version   Show version of this program

    Subcommand: run-service - Starts ${name} as a daemon that services HTTP requests
       -h, --help   Show help message
    ---

EXAMPLES
--------

    ${artifactId} -o value


INSTALLATION AND CONFIGURATION
------------------------------

### Installation steps

1. Unzip the tarball to a directory of your choice, typically `/usr/local/`
2. A new directory called ${artifactId}-<version> will be created
3. Add the command script to your `PATH` environment variable by creating a symbolic link to it from a directory that is
   on the path, e.g. 
   
        ln -s /usr/local/${artifactId}-<version>/bin/${artifactId} /usr/bin


### Configuration

General configuration settings can be set in `cfg/application.properties` and logging can be configured
in `cfg/logback.xml`. The available settings are explained in comments in aforementioned files.


BUILDING FROM SOURCE
--------------------

Prerequisites:

* Java 8 or higher
* Maven 3.3.3 or higher

Steps:

        git clone https://github.com/DANS-KNAW/${artifactId}.git
        cd ${artifactId}
        mvn install
