Change Log
=======

# 1.0.6 / 2014-06-19
## Changes
- Improved token handling in forwarder and http_status check.
- Updated the agent to allow plugins to override the default dimensions in the plugin config
- Added detection and auto-configuration of Nova, Swift and Cinder OpenStack processes and APIs
- Fixed crash in collector where plugins take more than 120 seconds to run
- Changed "active" plugins http_check, host_alive, and nagios_wrapper to use ServiceCheck class for threadpool support

# 1.0.5 / 2014-06-12
## Changes
- Initial support for mon-setup
- Changed project_id to project_name in the configuration

# 1.0.4 / 2014-06-09
## Changes
- host_alive and nagios_wrapper plugins can now support separate dimensions per instance

# 1.0.3 / 2014-05-28
## Changes
- Fixed http_check does not handle exception for unroutable network
- Fixed forwarder crashing with missing or malformed dimensions
- Removed deprecated "mon_" prefix from http_check metrics
- Fixed request format for Keystone token retrieval
- Changed supervisor to run as the mon-agent user, not root


# 1.0.2 / 2014-05-19
## Changes
- Integrated mon_client library
- Fixed bug in keystone processing

# 1.0.1 / 2014-05-12
## Changes
- Fixed subsequent dimensions missing in certain plugins

# 1.0.0 / 2014-04-28
## Changes
- Fork from Datadog agent 4.2.0
- removed most datadog branding
- removed embeded code
- Cleaned up name of collector/forwarder
- remove pup
- some pep8 changes, lots to go
- removed custom emitters
- removed data dog emitter, insert initial mon emitter
- collector only sends to forwarder now (previously you could optionally have it bypass the forwarder and send to datadogs)
- moved non-code files to root of project
- removed rpm build
- Rearranged code so things are more logically grouped
- Setup a standard message format for communicating to the forwarder
- Converted from tags to dimensions throughout the collector
- Rebranded dogstatsd and converted to dimensions
