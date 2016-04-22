# linux_scripts
## Possible problems while Installing gem on ubuntu

###When timeouts to repo
ex : ERROR:  While executing gem ... (Gem::RemoteFetcher::FetchError)
    Errno::ETIMEDOUT: Connection timed out - connect(2) for "api.rubygems.org" port 443 (https://api.rubygems.org/specs.4.8.gz)
####proxy problem
$gem install --http-proxy http://[proxy_ip]:[proxy_port] $gem_name

####ruby_dev does not exist
$sudo apt-get install ruby-dev

####ruby is not up to date
$gem update --system
