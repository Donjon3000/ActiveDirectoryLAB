<h1>Active Directory Lab</h1>



<h2>Description</h2>

<br />


<h2>Languages and Utilities Used</h2>



<h2>Environments Used </h2>

- <b></b> 

<h2>Program walk-through:</h2>

<p align="center">

First step is to downnload a Vitrual machine station ill will be using VM player for this lab

![vm player](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/ffb9d1ff-7de2-40d8-b39c-5a9efd270caf)

scroll down and choose whichever operating system you have. ill be using linux. Then click downlooad and save to downdlaods folder

![vmplayer linux](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/d4df0105-048a-4ae0-9413-31e2acb9c312)

Next is to download a windows server. search microsoft evaultion center and click microsoft server and choose the 2019 version

![microsoft ](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/0b225956-9538-497c-a0a4-50086833ff05)

click the download iso and fill out a register form 

![register](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/3b81e909-230b-4743-a02b-121d511f45ca)

after filling out the form download the 64 bit version and save it to your downloads folder

![2019 iso](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/418d62cd-5ef7-47bd-a237-3c096451db5a)

Now we can start setting up our vitrual machine 

![create vm](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/d40330ed-6bfb-43f5-ae86-118fc868e35c)

click install system later

![install later](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/74c73357-5c50-49b6-8a3a-5e9f4b8f7c42)

next click windows and then scroll down and select windows server 2019

![vm 2019](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/e665f565-3de2-4719-ab6d-d2f54743f017)

you can change the name of the server if you want to if not click next

![name whatever](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/cfab5b33-0ef5-4841-a448-02551c2e24db)

Have this set to split disk into mulitple files

![click next](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/33c804e1-f69b-4765-bf95-f2869b2bfc99)

CLick customize hardware and select new CD/DVD. select use new iso file and browse to your downloads and selected the windows 2019 iso the you dowladed earlier. click close and finish after your done

![hardware](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/e65a00e8-a5ea-4670-8d26-decf82d7380f)

now we can power up the VM by right clicking the windows server 2019 icon at the top left corner or simply clicking the power on button

![start machine](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/b00f679a-72ff-4e6b-872e-ff5623b93e87)

Now we can start setting up our windows virtual machine

![create new VM](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/b250ddc4-474e-4a13-8a9f-680141a5894f)

once you log in the the server manager should pop up 

![windows server](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/445a2f9b-1f38-4cb1-8f76-7de617f86560)

click on manage and then click add roles and feats

![roles and feats](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/1f5b5084-5d83-4c96-b4f6-61b43d3a189d)

Then select Role based installation 

![role based](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/7832420b-9ddb-4f42-a199-93cb374e6850)

click actvie directory services and clcick next then click add features

![domain](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/97cf2d7c-5e83-4a0d-8e3a-2bcf41ba8dc2)

click the install button once done dont click the close out button and instead click promote this server to a new domain controller

![dont click](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/596d44d0-1643-48e6-944d-be3a7e5a5be3)

Then select add new forest and name the doamin whatever you like

![AD local](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/7bb174e4-b47d-4196-8b54-db1de6d31eab)

then select the forest funcitonal level which will be windows 2016. create a password and make sure unclick then DNS option

![DC](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/851de2c0-cbdd-49ed-b364-64891702af2d)

then click next for the addtional options and click next for the defaults aswell

![additional options](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/77355bab-0a2c-41a7-bb6a-9a5ffa5f5bdb)

before installing the system will make sure you meet all the prerequistes. Once you see the green check mark you can click install

![pre check](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/33e2b670-2080-4a0b-8429-e7e961240342)

Once you hit install the VM will sign you out and will begin to restart. When you log back in you will see the domain name added with your admin user. thats how you know that the installation process worked

![new sign in](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/ca293eca-42ac-48f0-954b-fbfb020c66f3)

We have now successfully installed active directory on our virtual machine. Now got the tools and select Active Directory users and computers and you can see the domain name for out lab

![AD local 2](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/472f1d75-5ec7-4d8c-802c-56d2e47a14f1)

Now we can with the basics of active directory.The first thing we can do is create and Organizational Unit. 










































