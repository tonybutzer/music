down:
	wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
	mv Mini* /tmp

install:
	#mkdir /data2/$USER
	mkdir -p /home/conda/tmpconda
	#sudo chown -R ec2-user /data
	TMPDIR=/home/conda/tmpconda bash /tmp/Miniconda3-latest-Linux-x86_64.sh


docker:
	sudo yum install docker
	sudo usermod -aG docker ${USER}
	sudo systemctl enable docker
	sudo systemctl start docker


install-s3fs-centos:
	sudo yum install epel-release   # amazons version
	sudo yum install s3fs-fuse

