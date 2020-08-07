## K6 - A load testing tool for performance tuning of MicroService Application

### Use cases:
- Performance of the webserver 
- HTTP request/response with respect to predefined virtual users. 
- Integration with the CI/CD pipeline to check the botlleneck issue with new features, etc. 

### Installation 

Linux

For Debian-based Linux distributions, you can install k6 from the private deb repo like this:

``` 
sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 379CE192D401AB61
echo "deb https://dl.bintray.com/loadimpact/deb stable main" | sudo tee -a /etc/apt/sources.list
sudo apt-get update
sudo apt-get install k6
``` 

And for rpm-based ones like Fedora and CentOS:

``` 
wget https://bintray.com/loadimpact/rpm/rpm -O bintray-loadimpact-rpm.repo
sudo mv bintray-loadimpact-rpm.repo /etc/yum.repos.d/
sudo dnf install k6   # use yum instead of dnf for older distros
``` 

Docker

``` docker pull loadimpact/k6 ``` 

