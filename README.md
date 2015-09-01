nebula-clojure-plugin
==============
[![Build Status](https://travis-ci.org/nebula-plugins/projects/nebula-clojure-plugin.svg?branch=master)](https://travis-ci.org/nebula-plugins/projects/nebula-clojure-plugin)
[![Coverage Status](https://coveralls.io/repos/nebula-plugins/projects/nebula-clojure-plugin/badge.svg?branch=masterservice=github)](https://coveralls.io/github/nebula-plugins/projects/nebula-clojure-plugin?branch=master)
[![Gitter](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/nebula-plugins/projects/nebula-clojure-plugin?utm_source=badgeutm_medium=badgeutm_campaign=pr-badge)
[![Apache 2.0](https://img.shields.io/github/license/nebula-plugins/projects/nebula-clojure-plugin.svg)](http://www.apache.org/licenses/LICENSE-2.0)


Small wrapper around clojuresque, to avoid the including of clojars logic. We found that the clojars plugin. We're still
just applying the other core clojuresque plugins.

## Applying the Plugin

To include, add the following to your build.gradle

    buildscript {
      repositories { jcenter() }
      repositories { maven { url 'http://clojars.org/repo' } }

      dependencies {
        classpath 'com.netflix.nebula:nebula-clojure-plugin:2.2.+'
      }
    }

    apply plugin: 'nebula-clojure'

-or-

    buildscript {
    	repositories { maven { url 'http://clojars.org/repo' } }
    }

    plugins {
    	id 'nebula.nebula-clojure' version '2.2.0'
    }
