# Scan Matching Localization

## Project goal
- This project is to apply ICP and NDT for scan matching localization for 170 m from and keep the pose error to be less than 1.2 m. 

## Installation
- Used Udacity workspace 

## Run the project code

- Enable GPU Mode and connect to the virtual "Desktop". 
- Start two terminals in Desktop: one to run the Carla simulator by the commands:
```
su - student 
cd /home/workspace/c3-project
./run_carla.sh
```
- the second terminal to run the compiled project code with NDT by the commands:
```
./cloud_loc
```
- the second terminal to run the compiled project code with ICP by the commands:
```
./cloud_loc 2
```

- click on the viewer to activate listener, 
- tap the UP arrow key 3 times. It takes several seconds for the car to show the speed after tapping the key.

## Findings
- Increasing the number of iterations doesn't necessarily help. Iterations is set to 5 for both ICP and NDT for this effort to compare the performance.
- The NDT algorithm works better than the ICP algorithm with the parameters setting for this project. The Max error is 0.98 m for ICP and 0.61 m for NDT.
- The results snapshots are saved as ndt_passed.png and icp_passed.png for your information.

