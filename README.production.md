#puppet-site_data

#### Table of Contents

1. [Overview](#overview)
2. [Module Description - What the module does and why it is useful](#module-description)
4. [Usage - Configuration options and additional functionality](#usage)
5. [Reference - An under-the-hood peek at what the module is doing and how](#reference)
5. [Contributors - Who contributed](#contributors)
6. [Licence - Guide for contributing to the module](#development)

## Overview

This is a sample hiera directory to assit in bootstrapping R10K and Puppet.
We will utilize R10K's ability to consume the git Branch to populate our
puppetmaster properly with hiera.


## Module Description

This contains the example hiera data directory structure.

We will be utilzing git branches, R10K, and The Puppet Environments and Rolls concepts.
to dynamically create our data structure for puppet infrastructure.
See the references below for futher reading.  

The following Git branches exist within the repository.

    - Master      (The Master Branch )
    - production  ( Production Branch: Used for storing production values?)
    - development ( Development Branch: Data to support rapid development?)
    - testing     ( The Testing: QA and CI/CD data?)
    - staging     ( The Staging: Pre production data )


## Usage

Download and Edit Hiera within your development environment

  cd /usr/local/src
  git clone https://github.com/ppouliot/puppet-site_data.git

If you were to edit the repo now you would be editing the Master Branch.
To switch to a specific branch specify one of the names branch names above
replacing the name of the branch in the following command.

  git checkout production

To commit changes upstream use the following example as a guide replacing the name of the branch with the current branchname 

  git add *
  git commit -m "some changes to Production"
  git push origin production






## Reference

  url: https://docs.puppetlabs.com/puppet/latest/reference/environments.html
  url: http://sysadvent.blogspot.com/2012/12/day-13-configuration-management-as-legos.html
  url: http://garylarizza.com/blog/2014/03/07/puppet-workflow-part-3b/
  url: http://garylarizza.com/blog/2014/02/18/puppet-workflow-part-3/
  url: http://garylarizza.com/blog/2014/03/26/random-r10k-workflow-ideas/
  url: http://garylarizza.com/blog/2014/08/31/r10k-plus-directory-environments/

   
## Contributors

 * Peter Pouliot <peter@pouliot.net>

## Copyright and License

Copyright (C) 2014 Peter J. Pouliot

Peter Pouliot can be contacted at: peter@pouliot.net

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

  http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

/etc/puppet/modules/osticket/README.md (END)
