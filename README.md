# ansible-udemy-india

1. agar vagrant box bisa diremote input ip dan hostname pada /etc/hosts
   - sudo vi /etc/host

2. untuk bisa di remote copy ssh local PC to vagrant
   - cd ~/.ssh
   - ssh-keygen -t rsa
   - ssh-copy-id -i [letak ssh/dan nama file] vagrant@vagrant1 (copy di semua vagrant)

3. setting sudoers agar user vagrant mendapat privilege root tanpa password
   - sudo su -
   - echo "vagrant ALL=(ALL) NOPASSWD:ALL" >> /etc/sudoers

   note: setting di semua vagrantbox

4. rubah hostname di tiap vm edit masukkan /etc/hosts
   - sudo vi /etc/hosts
	- 127.0.0.1 vagrant1 
   - sudo hostnamectl set-hostname vagrant
   note: (sesuaikan nama host di tiap vm)

Ready to Learn :


