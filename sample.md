# AZURE VM CREATION
1. Login to azure account
2. Click on **search** **(1)**
   
   ![click on search](images/1.jpg)

3. Enter **virtual machines** **(1)** in the search and Under Services, select **Virtual machine** **(2)**.

   ![enter vm in serach](images/1.1.jpg)

4. In the Virtual machines page, select **Create** **(1)** on top left  and then click on **Azure virtual machine** **(2)**. The Create a virtual machine page opens.

   ![click on create](images/2.jpg)

5. Under **project details**, select subscription **(1)** `Innova8 Training` and create or select respective resource group **(2)** name `shiva.kumarmv`

   |Label|Name|
   |---|---|
   |Subscription|Innova8 Training|
   |Resource group| shiva.kumarmv|

   ![sub/rg](images/3.jpg)


6. Under **Instance details**, enter `windowsvm` for the Virtual machine name **(1)** and choose region **(2)** `east us`, in **availability option** select **availability zone**  and select `zone 1` in  **availability zone** **(3)**
   
   |Label|Name|
   |---|---|
   |Virtual machine name|windowsvm|
   |Region|east us|
   |availability option|availability zone |
   |availability zone| zone 1|

   ![instance details](images/4.jpg)

7. Choose `Windows Server 2022 Datacenter: Azure Edition - x64 Gen 2` for the **Image** **(1)**and select `Standard_DS1_v2` for **size** **(2)**. Leave the other defaults.

   |Label|Name|
   |---|---|
   |Image|Windows Server 2022 Datacenter: Azure Edition - x64 Gen 2|
   |Size|Standard_DS1_v2|

   ![image](images/5.jpg)

8. Under **Administrator account**, provide a **username** **(1)** , such as `azureuser` and a **password** **(2)** as `madhanshiva@12`. The password must be at least 12 characters long `Azure portal - between 12 - 123` characters.

   8.1 Under **Inbound port rules**, choose **Allow selected ports** and then select `RDP (3389)` from the drop-down of **select inbound ports** **(3)**.

   |Label|Name|
   |---|---|
   |username|azureuser|
   |password|madhanshiva@12|
   |Confirm Password| madhanshiva@12|
   |Indound rule|RDP (3389)|

   ![addmin name/pass](images/6.jpg)

9. Leave the remaining defaults and then select the `next - Disk` **(1)** button at the bottom of the page.

   ![confirm](images/7.01.jpg)
   
10. Under **os disk** , select the **os disk size** **(1)** `image default 127GB` and **os disk type** **(2)** `Standard SSD` and select **delete with vm** **(3)**

    |Label|Name|
    |---|---|
    |os disk size|mage default 127GB|
    |os disk type|Standard SSD|
    |delete with vm| :white_check_mark:|__--
   
    ![disk](images/7.jpg)

11. Leave the remaining defaults and then select the `next - Networking` **(1)** button at the bottom of the page.

    ![next](images/8.1.jpg)

12. under **Network Interface** , Choose an existing virtual network and subnet or create new ones. in this case **virtual network** **(1)** name  `windowsvm-vnet` and **subnet** **(2)** `10.3.0.0/24` and **public ip** **(3)** as `windowsvm-ip`

    |Label|Name|
    |---|---|
    |virtual network|windowsvm-vnet|
    |subnet|10.3.0.0/24|
    |public ip|windowsvm-ip|
    
    ![network](images/8.jpg)

13. Select the **delete public ip and nic when vm is deleted** **(1)** and leave the remaining defaults

    ![next](images/9.jpg)

14. Leave the remaining defaults and then select the `Review + create` **(1)** button at the bottom of the page.

    ![Review + create button](images/10.jpg)

15. After validation runs, select the `Create` **(1)** button at the bottom of the page

    ![create](images/11.jpg)

16. deploying resources

    ![deploy](images/12.jpg)

17. After deployment is complete, select `Go to resource` **(1)**.

    ![go](images/13.jpg)

18. On the overview page for your virtual machine, click on connect **(1)** and  select the `Connect` **(2)**
    

    ![connect](images/14.jpg)

19. Scroll down and click `Download RDP file` **(1)**.

    ![download](images/15.jpg)

20. GO to downloads and Open the `downloaded RDP file` and click `Connect` **(1)** when prompted

    ![connectrdp](images/16.jpg)

26.  Type the username `azureuser`, enter the password you created for the virtual machine in **password block** **(1)** , and then click **OK** **(2)**.

     ![username/pass](images/17.jpg)

27. You may receive a certificate warning during the sign-in process. Click **Yes** **(1)** or Continue to create the connection.

    ![cert](images/18.jpg)
    



