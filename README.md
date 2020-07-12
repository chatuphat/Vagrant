# Vagrant

Vagrant เป็น software ชนิดหนึ่งที่มีความสามารถการจัดการโปรแกรม Virtualization อย่างเช่น Virtualbox, Hypser-V ได้ โดยจุดเด่นของ Vagrant ก็คือเราสามารถสร้างเครื่อง Server เก็บไว้เป็น Box (Template) หากจะใช้งานเราก็สามารถสร้างเครื่อง Server ผ่านทาง file configuration ของ vagrant ได้เลย แบบรวดเร็วทันใจ

Start Building a Box

```
vagrant init ubuntu/bionic64
```

Config  Vagrantfile
```
config.vm.provider "virtualbox" do |v|
  v.memory = 2048  //mb
  v.cpus = 2 //core
end
```

Start Vagrant

```
vagrant up
```

Remote in SSH
```
vagrant ssh [name]
```

Restart
```
vagrant reload
```

Shut Down
```
vagrant halt
```
