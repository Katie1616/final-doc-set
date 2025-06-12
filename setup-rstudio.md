# Setting Up RStudio

> Setting up your RStudio will only need to happen once. You will need to install the packages to set up your application. 

1. In the files section in the bottom right hand corner, navigate to the MyFavoriteAlbums folder that you extracted the files from. 

  ![RStudio Files](/img/rstudio-files.png)
  
2. Click on the ‘app.R’ file. Your screen should now look like this. Note the console, which we will use in the coming steps. 
  
  ![RStudio Console](/img/rstudio-console.png)
  
3. In the console you will want to copy the following commands and press enter to “run” them. To give you access to the required libraries. 
        
        install.packages("shiny")
        install.packages("dplyr")
        install.packages("DT")
        install.packages("ggplot2")
  
  Your console should look like this after you installed the packages. If you encounter any issues please be sure that the code matches the code above exactly and there is no other additional text. 

  ![RStudio Package Installation](/img/rstudio-packages.png)

