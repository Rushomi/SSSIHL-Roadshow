![Screenshot 2024-12-15 191330](https://github.com/user-attachments/assets/cfab700c-b71e-45e5-bae3-3501869e6b9a)# SSSIHL-Roadshow


1. Open the ubuntu software from the oracle virtual box in windows
 ![Screenshot 2024-12-13 100421](https://github.com/user-attachments/assets/5690b11a-d717-481a-b6af-368104176789)
2. Open the terminal and Enter sudo apt install gedit
Then after the execution of the command enter the password as : vsdiat
now, Create a file called hello.c and enter the following code
![Screenshot 2024-12-13 190322](https://github.com/user-attachments/assets/dcd06d9a-e554-4ad8-8d87-7df0c40ce96b)

3. Now type gcc and enter the file name Eg:hello.c
and then enter the command ./a.out to execute the code
![Screenshot 2024-12-13 190547](https://github.com/user-attachments/assets/4632d539-ff69-4371-8a37-2f984ae0ab06)

4. After the execution enter the command "riscv64-unknown-elf-gcc -O1 -mabi=lp64 -march=rv64i -o hello.o hello.c" and execute, Now enter the following command "riscv64-unknown-elf-objdump -d hello.o" to see the following output
![Screenshot 2024-12-13 113003](https://github.com/user-attachments/assets/23408976-7d7b-40db-aa80-68e1f70fcbf2)

5. Now change directory to openlane flow directory using the command "cd Desktop/work/tools/openlane_working_dir/openlane"

Enter the command docker

After the execution of the above enter the command ./flow.tcl -interactive to see the following
![Screenshot 2024-12-13 121342](https://github.com/user-attachments/assets/0253f00a-0fa3-4b82-a4c0-843f83a66075)

6. Then enter the command "package require openlane 0.9".After execution enter the command "prep -design picorv32a" to get the following output.
![Screenshot 2024-12-13 122041](https://github.com/user-attachments/assets/e9d3d627-361b-4b12-9d6d-d08240557397)

7. Enter the following command "run_floorplan" and execute. 

![Screenshot 2024-12-13 123812](https://github.com/user-attachments/assets/ee14d425-f633-49ba-a4db-c48b71aae03a)

8. Enter the command "eog designs/picorv32a/runs/13-12_06-24/results/floorplan/picorva32a.floorplan.def.png" and execute.
![Uploading Screenshot 2024-12-13 191330.png…]()

9. Enter the command "run_placement" and execute,then enter the command "eog designs/picorv32a/runs/13-12_06-47/results/placement/picorva32a.placement.def.png"
![Screenshot 2024-12-13 191613](https://github.com/user-attachments/assets/6ffb9076-f9df-47e2-9f6b-f1d25c1d6884)

10. Enter the command "run_cts" and execute,then Enter the command "run_routing" and execute.
![Screenshot 2024-12-13 145140](https://github.com/user-attachments/assets/c6bf45f3-5382-4800-b68a-f224081ca90d)




