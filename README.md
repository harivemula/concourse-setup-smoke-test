# concourse-setup-smoke-test
Concourse CI - setup smoke test. Concourse setup using Bosh.
This assumes you have setup concourse with Bosh and it pulls concourse url from bosh when you login.
- Setup fly cli, run the below command and follow the instructions on console output
```
$ fly -t ci login
```
- Check if you are able to connect to concourse
```
$ fly -t ci builds
```
- Setup the inital test
```
$ fly -t ci set-pipeline -p test1 -c helloworld.yml
```
