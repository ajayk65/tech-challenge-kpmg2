Run below command in EC2 instance terminal. It is assumed that we have linux EC2
instance.

**1.** Install go using below two sub-steps.

wget -P /tmp https://golang.org/dl/go1.15.2.linux-amd64.tar.gz

sudo tar -C /usr/local -xzf /tmp/go1.15.2.linux-amd64.tar.gz

**2.**  Download the source file

wget https://github.com/ajayk65/kpmgtechchallenge2/blob/main/metadata.go

**3.** Execute go script as below to output meta-data on console in json format.  

go run metadata.go --prettyprint

**4.** Bonus point. To output particular data key use below command

go run metadata.go --prettyprint | grep \<data-key\>
