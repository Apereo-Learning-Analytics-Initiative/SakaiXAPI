SakaiXAPI
=========

This is mostly a pointer to the source code in the Sakai codebase that handles XAPI (TinCan) integration. I hope it is helpful to others who are trying to develop LRS integrations.

Files
-----
**LearningResourceStoreService.java** - The API which represents the XAPI LRS data objects and operations (statement transmit)

**LearningResourceStoreProvider.java** - A pluggable API to allow multiple LRS connections (implement this API for each type of LRS we are connecting to)

**BaseLearningResourceStoreService.java** - Sakai specific XAPI integration code which extracts the data

Main code location
------------------
Sakai main subversion repository location for kernel

    https://source.sakaiproject.org/svn/kernel/trunk/api/src/main/java/org/sakaiproject/event/api/
    https://source.sakaiproject.org/svn/kernel/trunk/kernel-impl/src/main/java/org/sakaiproject/event/impl/

NOTE
----
If you want to see the code which actually sends statements to the LRS then check out the project here:

    https://github.com/Apereo-Learning-Analytics-Initiative/SakaiXAPI-Provider
