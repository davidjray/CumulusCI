Key Concepts
============

The Product Development Model
-----------------------------
Salesforce DX helped define the common terminology of the `Org Development Model <https://trailhead.salesforce.com/en/content/learn/modules/org-development-model>`_ and the `Package Development Model <https://trailhead.salesforce.com/en/content/learn/modules/sfdx_dev_model>`_.
CumulusCI Suite enables the concept of the Product Development Model, an extension of the Package Development Model.
Salesforce.org products are made up of a collection of managed packages as well as pre-install and post-install automation to create usable environments for users.
There are a number of reasons products might choose to keep such configuration outside of the managed package itself.

* `Some metadata types are not packageable <https://developer.salesforce.com/docs/metadata-coverage>`_ in managed packages such as Standard Value Sets
* `Some metadata types have special behavior in managed packages <https://developer.salesforce.com/docs/atlas.en-us.packagingGuide.meta/packagingGuide/packaging_component_behavior.htm>`_ that might not be desirable
* Keeping some types of metadata outside the package can be used as an architectural choice to allow for flexibility in implementations

The Product Development Model aims to represent a holistic view of delivery of a product instead of simply releasing a package.


Projects
--------


Tasks and Flows
---------------
Tasks and Flows are the engine that power CumulusCI automation.
Tasks represent a single use action.
Flows allow you to define a sequence of either tasks or flows to execute in order. 
All Tasks and Flows are defined in the ``cumulusci.yml`` file.
