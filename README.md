<h1>Configuring and Displaying Speed, Duplex, and Description on a Swtich</h1>


 <h2>Description</h2>
In this lab, I learned to configure and display speed, duplex, and description on a switch. Switch interfaces that support multiple speeds (10/100 and 10/100/1000 interfaces), by default, will auto-negotiate what speed to use. However, you can configure the speed and duplex settings with the duplex {auto | full | half} and speed {auto | 10 | 100 | 1000} interface subcommands.
<br />

<h2>Languages and Utilities used</h2>

- <b>Putty</b>
- <b>ASA terminal</b>

<h2>Environments Used </h2>

- <b>Windows 10</b> 

<h2>Program walk-through:</h2>

<p align="center">
From the desktop, open PuTTY: <br/>
<img src="https://i.postimg.cc/mhfBCM2w/Screen-Shot-2022-06-17-at-3-52-11-PM.png" height="80%" width="80%" alt="Configuring and Displaying Speed, Duplex, and Description on a Swtich Steps"/>
<br />
  
  
<br />
In the PuTTY Configuration dialog box under the Saved Sessions section, double-click ASA:  <br/>
<img src="https://i.postimg.cc/0jtHq1hJ/Screen-Shot-2022-06-17-at-3-56-53-PM.png" height="80%" width="80%" alt="Configuring and Displaying Speed, Duplex, and Description on a Swtich Steps"/>
<br />
  
  
  
  
<br />
In the ASA terminal window, type admin@ASA's password as ******** and press Enter:  <br/>
<img src="https://i.postimg.cc/qq9yKm35/Screen-Shot-2022-06-17-at-4-00-27-PM.png" height="80%" width="80%" alt="Configuring and Displaying Speed, Duplex, and Description on a Swtich Steps"/>
<br />
  
  
  
<br />
In the ASA terminal window, execute command "en" to enter into enable mode:  <br/>
<img src="https://i.postimg.cc/x1781kL6/Screen-Shot-2022-06-17-at-4-02-37-PM.png" height="80%" width="80%" alt="Configuring and Displaying Speed, Duplex, and Description on a Swtich Steps"/>
<br />

  
  
<p align="center"> In the ASA terminal window, execute the following commands to configure IPv4 on a switch:
 <br>1. conf t</br>
 <br>2.interface GigabitEthernet 0/6</br>
 <br>3. duplex full</br>
 <br>4. speed 100</br>
 <br>5. description Printer on 3rd floor, preset to 100/full</br>
 <br>6.end</br>
 <br/>
<img src="https://i.postimg.cc/6pDZ1bb6/Screen-Shot-2022-06-17-at-4-10-37-PM.png" height="80%" width="80%" alt="Configuring and Displaying Speed, Duplex, and Description on a Swtich Steps"/>
<br />


<p align="center"> In the ASA terminal window, execute the following to show the IP configuration:
<br> 1. show running-config interface GigabitEthernet 0/6</br>
<br> 2. exit</br>
<br/>
<img src="https://i.postimg.cc/Jhsqsdtj/Screen-Shot-2022-06-17-at-4-19-58-PM.png" height="80%" width="80%" alt="Configuring and Displaying Speed, Duplex, and Description on a Swtich Steps"/>
<br />
  </p>
 
  
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
