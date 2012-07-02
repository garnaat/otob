otob
====

This is a simple sketch of how boto might look using requests rather
than httplib.

Clone this and make sure '.' is in your PYTHONPATH and then:

% cd otob
% python
>>> import otob.services.ec2
>>> c = otob.services.ec2.EC2Connection()
>>> c.describe_instances()

This should return a Python dict object containing the response data.