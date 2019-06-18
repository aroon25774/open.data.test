# An introduction to ROOT

![](.gitbook/assets/root.png)

CERN data is not easy to look at and analyze. The data files are in this format called Analysis Object Data or AOD for short. This is where the virtual machine and ROOT comes in handy. The virtual machine will stream the data while ROOT can allow for us to view the data. Without both the virtual machine and ROOT there would be no way of viewing the data files. Lets walkthrough how to use ROOT to view the data files!

{% hint style="danger" %}
The following code is linux. If you are unfamiliar with this code then we recommend taking a short and free interactive course to learn it fast. Here  is a link to the course:

 [https://www.codecademy.com/learn/learn-the-command-line](https://www.codecademy.com/learn/learn-the-command-line)
{% endhint %}

Lets make a datasets directory where we will download and store our data

1. Launch and run cernVM
2. On the home page or the Applications Menu you will find the option to open a browser in the Virtual Machine, click on the browser icon and launch a browser
3. Once the browser is launched go to Cerns Open Data Portal at the link  [http://opendata.cern.ch/](http://opendata.cern.ch/) or by simply looking it up
4. At the bottom of the page click on "datasets"
5. Find your desired dataset 

Enter the following commands into your terminal to get started

```bash
$ cmsrel CMSSW_5_3_32 #This ensures you have the version of CMSSW running
$ cd CMSSW_5_3_32/src/ #This changes your directory to the source file
$ cmsenv #This makes sure you have a CMS environment
```

In order to root a file you need the file link on the virtual machine

