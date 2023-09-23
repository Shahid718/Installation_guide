# **Installing Dislin 11.5 ( Windows 10 )**

The steps below demonstrate how to update to the latest Dislin version. It has following main parts:

* Download and install Dislin distribution
* Configuration of the system
* Testing the installation
* Compiling double precision module


## **Download and installation**
1. Navigate to the link:

https://www.dislin.de/index.html

2. Click **Downloads**.

![Output](images/dislin_home.PNG)


3. Select **Distributions**

![Output](images/dislin_distribution.PNG)


4. Choose **Windows 64 bit**

![Output](images/dislin_windows_64.PNG)


5. Find the **distribution** for windows.

![Output](images/dislin_distribution_Mingw.PNG)


6. The dislin is downloaded in the **Download folder** 

![Output](images/dislin_download.PNG)

7. **Extract** it there. 

![Output](images/dislin_extract.PNG)

8. Open the **extract folder** and click **setup.exe**. 

![Output](images/dislin_setup.PNG)


9. The following window will appear. Click **OK**.

![Output](images/dislin_setup_window.PNG)


10. The following default setting will appear. Click **OK**. **Note:** This installation directory must be different from the temporary working directory.

![Output](images/dislin_installation_c.PNG)


11. The installation takes a while. Once **installation is done**, the dislin directory looks like. 

![Output](images/dislin_installed.PNG)

## **Configuration of the system**


12. Go to **control panel** and click **System**. 

![Output](images/control_panel_home.PNG)


13. Select **Advanced system settings**. 

![Output](images/control_panel_settings.PNG)


14. Check **Environment Variables**. 

![Output](images/system_properties.PNG)


15. Click **New** and Enter **variable name** and **variable value** under **System Variable**. 

![Output](images/edit_system_variable.PNG)


16. Under **path** make **New path** as **C:\dislin\win**. 

![Output](images/system_path.PNG)


## **Dislin test**


Go to the folder **C:\dislin\gf** and see the files **dislin.mod** and **dislin.o**. If the compiled files are not present, compile the **dislin.f90** file with the command

    gfortran -c dislin.f90


Go to the folder **c:\dislin\examples** and enter **f90link -a exa_f90**

![Output](images/cmd_example.PNG)


17. It shows the options for output

![Output](images/dislin_example.PNG)


18. Enter **cons**. It shows following options. Enter **1**

![Output](images/dislin_cons.PNG)


19. The output shows the **curve** on console.

![Output](images/dislin_curve.PNG)


20. The output also shows the **dislin information** on console. Try other examples.

![Output](images/dislin_information.PNG)


## **Double precision module**

By default dislin is single precision. To use double  precsion go to the folder **C:\dislin\gf\real64** and compile the file **dislin.f90** with command

    gfortran -c dislin.f90

![Output](images/congratulations.jpg)


---

**Date : 24 September 2023**
