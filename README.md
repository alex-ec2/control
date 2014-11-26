#### ec2tools download :
```
wget http://s3.amazonaws.com/ec2-downloads/ec2-api-tools.zip
unzip ec2-api-tools.zip
mv ec2-apt-tools* ec2-apt-tools
```

#### add to bottom of .bashrc
```
export JAVA_HOME="/usr/lib/jvm/java-7-openjdk-amd64/jre"
export EC2_HOME=/home/ec2/ec2-api-tools
export PATH=$PATH:~/bin:$EC2_HOME/bin
export AWS_ACCESS_KEY=your-aws-access-key-id 
export AWS_SECRET_KEY=your-aws-secret-key
```

#### verify
```
ec2-describe-regions
```

#### added current region end-point to .bashrc
```
export EC2_URL=https://ec2.us-east-1.amazonaws.com
```
