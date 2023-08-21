<h1>Active Directory Lab</h1>



<h2>Description</h2>
In this walkthrough we will be going through the process of installing an configurinfg Active Directory on a virtural machine and implement basic parctices that are used in a work enviorment.
<br />


<h2>Languages and Utilities Used</h2>
VM Player workstation Active Directory


<h2>Environments Used </h2>

Kali Linux <b></b> 

<h2>Program walk-through:</h2>

<p align="center">

First step is to downnload a Vitrual machine station ill will be using VM player for this lab.

![vm player](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/ffb9d1ff-7de2-40d8-b39c-5a9efd270caf)

Scroll down and choose whichever operating system you have. ill be using linux. Then click downlooad and save to downdlaods folder.

![vmplayer linux](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/d4df0105-048a-4ae0-9413-31e2acb9c312)

Next is to download a windows server. Search Microsoft Evaluation Center and click microsoft server and choose the 2019 version.
![microsoft ](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/0b225956-9538-497c-a0a4-50086833ff05)

Click the download iso and fill out a register form. 

![register](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/3b81e909-230b-4743-a02b-121d511f45ca)

After filling out the form download the 64 bit version and save it to your downloads folder.

![2019 iso](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/418d62cd-5ef7-47bd-a237-3c096451db5a)

Now we can start setting up our vitrual machine. 

![create vm](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/d40330ed-6bfb-43f5-ae86-118fc868e35c)

Click install system later.

![install later](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/74c73357-5c50-49b6-8a3a-5e9f4b8f7c42)

Next click windows and then scroll down and select windows server 2019.

![vm 2019](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/e665f565-3de2-4719-ab6d-d2f54743f017)

You can change the name of the server if you want to if not click next.

![name whatever](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/cfab5b33-0ef5-4841-a448-02551c2e24db)

Have this set to split disk into mulitple files.

![click next](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/33c804e1-f69b-4765-bf95-f2869b2bfc99)

Click customize hardware and select new CD/DVD. Select use new iso file and browse to your downloads and selected the windows 2019 iso the you dowladed earlier. Click close and finish after your done.

![hardware](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/e65a00e8-a5ea-4670-8d26-decf82d7380f)

Now we can power up the VM by right clicking the windows server 2019 icon at the top left corner or simply clicking the power on button.

![start machine](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/b00f679a-72ff-4e6b-872e-ff5623b93e87)

Now we can start setting up our windows virtual machine.

![create new VM](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/b250ddc4-474e-4a13-8a9f-680141a5894f)

Once you log in the the server manager should pop up. 

![windows server](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/445a2f9b-1f38-4cb1-8f76-7de617f86560)

Click on manage and then click add roles and feats.

![roles and feats](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/1f5b5084-5d83-4c96-b4f6-61b43d3a189d)

Then select role based installation. 

![role based](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/7832420b-9ddb-4f42-a199-93cb374e6850)

Click actvie directory services and click next then click add features.

![domain](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/97cf2d7c-5e83-4a0d-8e3a-2bcf41ba8dc2)

Click the install button once done dont click the close out button and instead click promote this server to a new domain controller.

![dont click](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/596d44d0-1643-48e6-944d-be3a7e5a5be3)

Then select add new forest and name the doamin whatever you like.

![AD local](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/7bb174e4-b47d-4196-8b54-db1de6d31eab)

Then select the forest funcitonal level which will be windows 2016. Create a password and make sure unclick then DNS option

![DC](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/851de2c0-cbdd-49ed-b364-64891702af2d)

Then click next for the addtional options and click next for the defaults aswell.

![additional options](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/77355bab-0a2c-41a7-bb6a-9a5ffa5f5bdb)

Before installing the system will make sure you meet all the prerequistes. Once you see the green check mark you can click install.

![pre check](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/33e2b670-2080-4a0b-8429-e7e961240342)

Once you hit install the VM will sign you out and will begin to restart. When you log back in you will see the domain name added with your admin user. Thats how you know that the installation process worked.

![new sign in](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/ca293eca-42ac-48f0-954b-fbfb020c66f3)

We have now successfully installed active directory on our virtual machine. Now got the tools and select Active Directory users and computers and you can see the domain name for out lab.

![AD local 2](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/472f1d75-5ec7-4d8c-802c-56d2e47a14f1)

 We can start with the basics of active directory.The first thing we can do is create and Organizational Unit. First click on the ADdomain then right click it. select new then select Organizational Unit.

![OU](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/b98d1073-1c6e-42a3-975e-eadaa8501555)

You can name the OU whatever you want it to be I decicded to name mine locations.

![OU in OU](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/731ab8c4-8d26-4d15-89ef-6f837974b406)

We can also create an OU inside an OU. Click the location OU and make sure its highlighted. Then click the yellow folder with the orange star. Where going to create four different OUs under the location OU. In this order create a computer, Distribution Group , users , and Security Group.

![Computer OU](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/cfcd2eba-b60c-4d1a-9124-8dc5b35f013b)

It should look like this when done.

![multi OUs](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/21e55f73-1bc0-44d1-9eef-5a4c715315a0)

Now will make even more OUs insides the OUs we just made before. For Computer create Server and Workstations. For Users create Accounting , HR , Engineering , Sales and Termed (stands for terminated). For Security Group create Payroll , IT , Onboarding , Contracts and Sales.

![more OUs](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/221a7071-1aa3-4db3-b7a6-aff465ba2af6)

Next we can create Users inside and OU. Click the OU User then right click it then select New then select user.

![new user](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/133ea53f-f5c5-4f7b-a135-05a8d70eaa0a)

Fill out the first and last name sections and create a unique user. Then click next and create a password. Then click next and finish.

![active user](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/5c8dacab-7264-4f03-9f5b-e1b0afcf5def)

Next we will create different groups in active directory. CLick security groups then Right click IT OU then select new then select group and we will name this Domain Admin.

![new IT group](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/5eac1d1e-e3f4-47c9-8acf-1a9d48b289e4)

Now lets practice finding a user in active directory by right clicking the Admin OU and click find.

![find](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/765c53bc-b0b3-40fb-b7b9-2368e312868d)

Type in the name of the user that you are looking for. 

![find user](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/057bdc3a-f3cc-44ce-902f-4e7f32b7cf59)

Let add a user to a security group. By doing the same process as before but now click memeber of and then click add. Then type the group you want the user to be apart example will type HR new hire.

![new  HR](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/a9ab5045-7573-4543-82cf-b3ca7d618ab2)

You can also remove a user from a group as well.

![add or remove](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/5f641a6c-2e56-4c78-9eb4-f7c3da1af1ff)

Now will practice enabling and disabling users accounts. Go back to Admin folder and find the user then right click the user name then select move then put the user in the termedniated folder.

![term folder](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/9fbea204-d58e-425d-b1b9-eb1d16fb9c62)

Then right click the user and select disable. And if you need to enable the account again just simply right click the user and select enable.

![disable](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/a9644779-f256-4e79-a796-f6620445006f)

if you need reset a users password just right click the user and select reset password and give them a temporary password.

![reset password](https://github.com/Donjon3000/NessusTenableLab/assets/140426313/d077660f-3674-46c2-94dc-10d6d1a57324)






