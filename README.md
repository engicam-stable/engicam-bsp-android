# ENGICAM BSP ANDROID

To get the BSP you need to have repo installed and use it as:

Install the repo utility:

    $: mkdir ~/bin
    $: curl https://storage.googleapis.com/git-repo-downloads/repo > ~/bin/repo
    $: export PATH=${PATH}:~/bin

Download the BSP source:

    $: PATH=${PATH}:~/bin
    # By default, after preceding command finishes execution, current working directory changed to the i.MX Android source code root directory.
    # ${MY_ANDROID} will be refered as the i.MX Android source code root directory in all i.MX Andorid release documentation.
    $: export MY_ANDROID=`pwd`
    $: repo init -u https://github.com/engicam-stable/engicam-bsp-android.git -b ${android-branches} -m engicam-imx-android-12.0.0_1.0.0.xml
    $: repo sync

| android-branches |      modules       |         Carrier         |
|:----------------:|:------------------:|:-----------------------:|
|                  |                    |                         |
|  imx-android-12  |  i.Core MX8M Plus  |  EDIMM 2.0 STARTER KIT  | 
|                  |  i.Core MX8M Mini  |                         |

