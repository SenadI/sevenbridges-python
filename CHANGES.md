0.9.5 (2017-10-12)
==================
- Bugfixes:
  - [Issue #98](https://github.com/sbg/sevenbridges-python/issues/98)
  - [Issue #99](https://github.com/sbg/sevenbridges-python/issues/99)
  
- Full support for AA features.
  
0.9.4 (2017-09-29)
==================
- Maintenance sleeper now retries on JsonDecode errors up to 15 seconds. (3x5s)

0.9.3 (2017-09-04)
==================
- Fix broken py2 compatibility
- Improve requirement handling for setup.py
- Fix `__eq__` method (yet again)

0.9.2 (2017-08-30)
==================
- Fix `__eq__` method for main resources.

0.9.1 (2017-08-23)
==================
- Fix small bug for interruptible instances.

0.9.0 (2017-08-22)
==================
- Added support for managing volume permissions.
- Added support for listing volume content.
- Added support for interruptable instances
- Added support for Enterprise account features.
- Added support for Advance Access Features
  Note that now all Advance Access features will be only enabled if its
  specified on the config level or explicitly when instantiating API object.
- All resources now implement deepcopy method to provide a way to copy an resource instance.
- `__eq__` method overridden on first level models (project, tasks etc) to allow easy comparision and enable `in` operator for Collection resources.
- Added primitive file content methods that downloads file and retrieves content.
- Update requests version 2.18.3.
- Documentation is updated to reflect new changes.
- Multiple tests added for both old and new resources.

- Backwards incompatible changes
  - Duration of download/upload is not in milliseconds.
  - `copy` method is removed from Input/Output model.

- Bugfixes
  - [Issue #93](https://github.com/sbg/sevenbridges-python/issues/93)


0.8.1 (2017-07-10)
==================
- Added documentation on how to query public apps.
- Added marker documentation.
- Fixed missing query params from apps query.

0.8.0 (2017-07-07)
==================
- Added Contributors notice.
- Added Actions service calls. Users are now able to send feedback to Sevenbridges and bulk copy files. Tests included.
- Added markers service calls. Users are now able to set,get,modify and delete markers on bam files. Advance Access feature - Possibility to be changed in the future.
- Volume modifications. Added volume permissions calls and possibility to deactivate volume.
- Travis setup.

- Bugfixes
  - [Issue #80](https://github.com/sbg/sevenbridges-python/issues/80)
  - [Issue #81](https://github.com/sbg/sevenbridges-python/issues/81)
  - [Issue #82](https://github.com/sbg/sevenbridges-python/issues/82)
  - [Issue #84](https://github.com/sbg/sevenbridges-python/issues/84)
  - [Issue #86](https://github.com/sbg/sevenbridges-python/issues/86)
  - [Issue #88](https://github.com/sbg/sevenbridges-python/issues/88)

0.7.4 (2017-05-13)
==================
- Bugfixes
  - [Issue #72](https://github.com/sbg/sevenbridges-python/issues/72)
  - [Issue #75](https://github.com/sbg/sevenbridges-python/issues/75)a
  - [Issue #77](https://github.com/sbg/sevenbridges-python/issues/77)
  - [Issue #78](https://github.com/sbg/sevenbridges-python/issues/78)

0.7.3 (2017-04-18)
==================
- Instance limit information added.
- Expanded task execution resource to reflect limit information.

- Bugfixes
  - [Issue #70](https://github.com/sbg/sevenbridges-python/issues/69)
  - [Issue #69](https://github.com/sbg/sevenbridges-python/issues/69)
  - [Issue #68](https://github.com/sbg/sevenbridges-python/issues/68)
  - [Issue #67](https://github.com/sbg/sevenbridges-python/issues/68)

0.7.2 (2017-03-30)
==================
- Add option to add users to project using email.

0.7.1 (2017-03-21)
==================
- Copy only feature for volumes advance access

0.7.0 (2016-02-10)
==================
- Changes in the library configuration. The location and format of the configuration files
has changed. This makes this version backwards incompatible. For information
regarding where to place new configuration, the names of the variables and the usage
can be found within documentation.
- Add logging for resource and http client.
- Add option to query files using tags.
- Add option to query tasks by timestamps.
- Add parameter to file save method to control if error should be raised.
- Add additional tests.


- Bugfixes
  - [Issue #64](https://github.com/sbg/sevenbridges-python/issues/64)
  - [Issue #63](https://github.com/sbg/sevenbridges-python/issues/63)
  - [Issue #62](https://github.com/sbg/sevenbridges-python/issues/62)
  - [Issue #61](https://github.com/sbg/sevenbridges-python/issues/61)
  - [Issue #56](https://github.com/sbg/sevenbridges-python/issues/56)
  - [Issue #55](https://github.com/sbg/sevenbridges-python/issues/55)
  - [Issue #54](https://github.com/sbg/sevenbridges-python/issues/54)
  - [Issue #53](https://github.com/sbg/sevenbridges-python/issues/53)
  - [Issue #49](https://github.com/sbg/sevenbridges-python/issues/49)


0.6.1 (2016-10-19)
==================
Removing duplicated error handlers that occur during api object
instantiation.

0.6.0 (2016-10-17)
==================

Added support for error_handlers. Users can now register error_handlers
that will be executed upon each request. 

- Bugfixes
  - [Issue #45](https://github.com/sbg/sevenbridges-python/issues/45)
  - [Issue #46](https://github.com/sbg/sevenbridges-python/issues/46)



0.5.4 (2016-09-30)
==================
- Bugfixes
  - [Issue #42](https://github.com/sbg/sevenbridges-python/issues/42)
  - [Issue #43](https://github.com/sbg/sevenbridges-python/issues/43)



0.5.3 (2016-09-23)
==================
- Bugfixes
  - [Issue #40](https://github.com/sbg/sevenbridges-python/issues/40)
  - [Issue #41](https://github.com/sbg/sevenbridges-python/issues/41)



0.5.2 (2016-09-15)
==================
- Bugfixes
  - [Issue #35](https://github.com/sbg/sevenbridges-python/issues/35)
  - [Issue #39](https://github.com/sbg/sevenbridges-python/issues/39)
  

0.5.1 (2016-08-29)
==================
- Bugfixes
  - [Issue #28](https://github.com/sbg/sevenbridges-python/issues/28)
  
0.5.0 (2016-08-29)
==================

- Project settings available on project resource. These settings
  can be currently used to create locked projects.
- File now have tags. User is able to view/set/edit tags.
- Support for proxies. User can now configure library to use proxies.


- Bugfixes
  - [Issue #30](https://github.com/sbg/sevenbridges-python/issues/30)
  - [Issue #29](https://github.com/sbg/sevenbridges-python/issues/29)
  - [Issue #28](https://github.com/sbg/sevenbridges-python/issues/28)
  - [Issue #24](https://github.com/sbg/sevenbridges-python/issues/24)
  - [Issue #23](https://github.com/sbg/sevenbridges-python/issues/23)
  - [Issue #14](https://github.com/sbg/sevenbridges-python/issues/14)


0.4.4 (2016-08-19)
==================
- Upload changes
  Upload sync/asyc returns the upload handle. The uploaded file 
  is available by invoking .result() method.
- Query optimizations
  All queries except those on app resource are not optimized using
  the _fields=_all query parameter.
- Bugfixes
    - [Issue #21](https://github.com/sbg/sevenbridges-python/issues/21)
    - [Issue #22](https://github.com/sbg/sevenbridges-python/issues/22)

0.4.3 (2016-08-12)
==================
- Bugfixes
    - [Issue #16](https://github.com/sbg/sevenbridges-python/issues/16)
    - [Issue #17](https://github.com/sbg/sevenbridges-python/issues/17)
    - [Issue #18](https://github.com/sbg/sevenbridges-python/issues/18)

0.4.2 (2016-07-27)
==================
- Bugfixes
    - [Issue #12](https://github.com/sbg/sevenbridges-python/issues/12)

0.4.1 (2016-07-27)
==================
- Bugfixes
    - [Issue #10](https://github.com/sbg/sevenbridges-python/issues/10)
    - [Issue #11](https://github.com/sbg/sevenbridges-python/issues/11)

0.4.0 (2016-07-18)
==================
- Introducing support for Volumes API
- Downloader refactor.
- Task statistics now carries docker information.
- Breaking compatibility on job.logs model because of newly added support for custom logs.
  job.logs behaves as a dictionary.
- Refactor .get query members to use resources and not construct the response on their own.
- Useful enums available in models.enums.
- Transformers now validate for Resource instances or strings. Everything else raises exception.

0.3.0 (2016-06-20)
==================

- Introducing file upload
- Fixing bug related to object reload.

0.2.0 (2016-05-30)
==================

-   Documentation cleaning.
-   Breaking compatibility on compound fields now they are dicts if declared as writable.
-   Bug fixes
  - [Issue #1](https://github.com/sbg/sevenbridges-python/issues/1)
  - [Issue #2](https://github.com/sbg/sevenbridges-python/issues/2)
  - [Issue #3](https://github.com/sbg/sevenbridges-python/issues/3)


0.1.1 (2016-04-27)
==================

-   Doc fixes
-   Changes in error decorator to throw Value Error due to py2-py3 compatibilty.


0.1.0 (2016-04-27)
==================

-   initial release

