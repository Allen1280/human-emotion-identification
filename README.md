# human-emotion-identification
Nvidia project_human-emotion-identification
Project goal:
Training an Ai to read human emotions by using data given to it.
During this project I have trained an Ai to predict the emotions that I make.
Project was done on July 13, 2023 in MIT. During the project, we learned that Ais are programmed to use human given data to make predictions.


## The Algorithm
The first part of the algorithm starts at the Jetson nano, Nvidia.
setup

1. Open the windows symbol at the bottom left corner (windows).

2. Type in “putty” and press the enter key, and use serial (speed 9600) not SSH (port 22),and find your communications (COM) and the number of it, once you have found it, login.

3. Login using “nvidia” and “nvidia” for both password and username.

4. Once you have logged in, type the command “nmcli device” and check to see if you're on wifi. Once you find you're not connected, use ‘nmcli device wifi’ to find your wifi, if it is not there follow the next step.

4a. If not then open up wifi and make sure that “share my internet connection with other devices” is (on).

4b. If your internet does not auto connect use the command “sudo nmcli --ask device wifi connect 'internet name’” on your putty. Then type in the password for the putty and then the password for your wifi network.

5. Once you are connected with the wifi use the command ‘ifconfig’ to find your ip address, it should either be wlan0, or etho0. Your ip address should be something like this exd,efx,eds,tgf. But with numbers.

6. After you have found your ip address you copy it with right click.

7. Open another putty but use SSH and add in your ip address, do the same login and password 
‘Nvidia’. Then download docker by using the following commands, ‘mkdir -p ~/nvdli-data’, ‘echo "sudo docker run --runtime nvidia -it --rm --network host \
    --volume ~/nvdli-data:/nvdli-nano/data \
    --device /dev/video0 \
    nvcr.io/nvidia/dli/dli-nano-ai:v2.0.2-r32.7.1" > docker_dli_run.sh’, ‘chmod +x docker_dli_run.sh’. (this may take a while depending on your wifi speed.
    

8. Then type the command ‘./docker_dli_run.sh’ to run jupyterlabs.

9. However, be advised that for some computers the link is given by the putty so if that is you, just type your ip address + : + ‘8888’. Once that is done use the passcode given by the putty device used on SSH.

10. Once in juypter labs, click on the folder classifications. And open it, you are now in the right place to begin the tests.
 

## Running this project

1. Everything is set up for you already
2. Change tasks and categories to emotions by adding # infront of the categories and tasks as well as a space, then=n remove the # and space of the previous selected category and task. This is important as it may jeopardize the computer and its controls.
3. You are set to run the tests.
[View a video explanation here](video link)
C:\Users\Student\Documents\Zoom


