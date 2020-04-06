# Jenkins Pipeline script for CI job

Please find the steps for integration for the same.

## Jenkins installation on Centos 7
```bash
wget -O /etc/yum.repos.d/jenkins.repo http://pkg.jenkins.io/redhat-stable/jenkins.repo
rpm --import http://pkg.jenkins.io/redhat-stable/jenkins.io.key
yum install jenkins java-1.8.0-openjdk –y
systemctl start jenkins
systemctl enable jenkins
```

##Add the following in the sudoers file [sudo visudo -f /etc/sudoers]
jenkins ALL=(ALL) NOPASSWD: ALL

## Installation

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install foobar.

```bash
pip install foobar
```

## Usage

```python
import foobar

foobar.pluralize('word') # returns 'words'
foobar.pluralize('goose') # returns 'geese'
foobar.singularize('phenomena') # returns 'phenomenon'
```

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)
