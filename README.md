# Thoth's Source Management
This library provides abstraction that allow's [thoth](https://thoth-station.ninja/) to interact with various source management systems.
We use OGR underneath to interact with git forges. 

## Install
Use pipenv - 
This project is released on
[PyPI](https://pypi.org/project/thoth-common), so the latest release can be
installed via pip or [Pipenv](https://pipenv.readthedocs.io) as shown below:

`pipenv install thoth-sourcemanagement`


## How to use - 
```python
from sourcemanagement.sourcemanagement import SourceManagement
from sourcemanagement.enums import ServiceType

# Service type you want to use
service_type = ServiceType.GITHUB
sm = SourceManagement(service_type, 'https://www.github.com', `private_token', 'username/repo_name')
```
You could then call all the functions offered by the Source Management class.