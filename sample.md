# AZURE VM CREATION
1. Login to azure account
2. Click on **search**
   
   ![click on search](images/1.jpg)

3. Enter **virtual machines** in the search and Under Services, select **Virtual machine**.

   ![enter vm in serach](images/1.1.jpg)

4. In the Virtual machines page, select **Create** and then **Azure virtual machine. The Create a virtual machine page opens.

   ![click on create](images/2.jpg)

5. Under **project details**, select subscription `Innova8 Training` and respective resource group name `shiva.kumarmv`

   |Label|Name|
   |---|---|
   |Subscription|Innova8 Training|
   |Resource group| shiva.kumarmv|

   ![sub/rg](images/3.jpg)


6. Under **Instance details**, enter `windowsvm` for the Virtual machine name and choose region `east us` and in availability option select availability zone  and select `zone 1`
   
   |Label|Name|
   |---|---|
   |Virtual machine name|windowsvm|
   |Region|east us|
   |availability option|availability zone |
   |availability zone| zone 1|

   ![instance details](images/4.jpg)

7. Choose `Windows Server 2022 Datacenter: Azure Edition - x64 Gen 2` for the Image and select `Standard_DS1_v2` for size. Leave the other defaults.

   |Label|Name|
   |---|---|
   |Image|Windows Server 2022 Datacenter: Azure Edition - x64 Gen 2|
   |Size|Standard_DS1_v2|

   ![image](images/5.jpg)

8. Under **Administrator account**, provide a **username**, such as `azureuser` and a **password** as `madhanshiva@12`. The password must be at least 12 characters long `Azure portal - between 12 - 123` characters.

   8.1 Under **Inbound port rules**, choose **Allow selected ports** and then select `RDP (3389)` from the drop-down.

   |Label|Name|
   |---|---|
   |username|azureuser|
   |password|madhanshiva@12|
   |Confirm Password| madhanshiva@12|
   |Indound rule|RDP (3389)|

   ![addmin name/pass](images/6.jpg)

9. Leave the remaining defaults and then select the `next - Disk` button at the bottom of the page.

   ![confirm](images/7.01.jpg)
   
10. Under **os disk** , select the **os disk size** `image default 127GB` and **os disk type** `Standard SSD` and select **delete with vm**

    |Label|Name|
    |---|---|
    |os disk size|mage default 127GB|
    |os disk type|Standard SSD|
    |delete with vm| :white_check_mark:|__--
   
    ![disk](images/7.jpg)

11. Leave the remaining defaults and then select the `next - Networking` button at the bottom of the page.

    ![next](images/8.1.jpg)

12. under **Network Interface** , Choose an existing virtual network and subnet or create new ones. in this case **virtual network** name  `windowsvm-vnet` and **subnet** `10.3.0.0/24` and **public ip** as `windowsvm-ip`

    |Label|Name|
    |---|---|
    |virtual network|windowsvm-vnet|
    |subnet|10.3.0.0/24|
    |public ip|windowsvm-ip|
    
    ![network](images/8.jpg)

13. Select the **delete public ip and nic when vm is deleted**  and leave the remaining defaults

    ![next](images/9.jpg)

18. Leave the remaining defaults and then select the `Review + create` button at the bottom of the page.

    ![Review + create button](images/10.jpg)

19. After validation runs, select the `Create` button at the bottom of the page

    ![create](images/11.jpg)

20. deploying resources

    ![deploy](images/12.jpg)

21. After deployment is complete, select `Go to resource`.

    ![go](images/13.jpg)

22. On the overview page for your virtual machine, click on connect and  select the `Connect`

    ![connect](images/14.jpg)

23. Scroll down and click `Download RDP file`.

    ![download](images/15.jpg)

24. GO to downloads and Open the `downloaded RDP file` and click `Connect` when prompted

    ![connectrdp](images/16.jpg)

25.  Type the username `azureuser`, enter the password you created for the virtual machine, and then click OK.

     ![username/pass](images/17.jpg)

26. You may receive a certificate warning during the sign-in process. Click Yes or Continue to create the connection.

    ![cert](images/18.jpg)
    



