# ElevatorControlWithFuzzyLogic
Elevator group control system using fuzzy logic triangular membership function

In this project i've made a elevator group control system using fuzzy logic. Elevator groups are normally used in commercial buildings and their control can be carried out in different ways, for instance by using the nearest elevator for attending the hall calls or by using a selection process, which evaluates multiple criteria 
in order to compute the most suitable elevator.From this point of view, the main objective of this work is the analysis and application of fuzzy control techniques in order to define the attribution of elevator priorities for attending the hall calls. . This work considers a Destination Control System and load capasity, which provides the control system with an a-priori knowledge of the desired floor for each hall call.

First ol all create the variables. Three of them are input variable and priority is output for fuzzy logic:

![variables](https://user-images.githubusercontent.com/43918312/146545104-8dfb7f14-72e5-4aa0-9e2b-b17caeaae465.PNG)

After that create membership functions:

![membership_function](https://user-images.githubusercontent.com/43918312/146545581-727d8ee1-8a4e-4ab6-83ef-e1f9b344a8b3.PNG)

After creating membership functions vitualize data:

![data_visualization](https://user-images.githubusercontent.com/43918312/146546183-375ec85d-106e-437c-b533-532f149f7772.PNG)

These are the pngs of input and output graphics of fuzzy logic steps:

1-) Waiting Time:

![waiting_time](https://user-images.githubusercontent.com/43918312/146546511-37cb19a9-b4b5-4455-8771-f6b9db30bd47.PNG)

2-) Distance:

![distance](https://user-images.githubusercontent.com/43918312/146546554-b64ae0d3-6fc9-467c-bca9-f5cb6b57150d.PNG)


3-) Load Capacity:

![load_capacity](https://user-images.githubusercontent.com/43918312/146546606-c4bec165-f2e5-45db-a8c6-9b8691255704.PNG)


4-) Priority:

![priority](https://user-images.githubusercontent.com/43918312/146546630-e32ca3df-6a13-412d-a415-74ecef8d3d38.PNG)

After these steps input your information. In reality these infos can be taken by IA.But in this project you have to write your own information.

![your_infos](https://user-images.githubusercontent.com/43918312/146547079-33ed37b5-8704-4628-b0c7-f3d261db45e9.PNG)

Elevator informations are taken in this section. Here have some calculation steps. Actually, we calculate waiting time in here. 

![elevator_infos](https://user-images.githubusercontent.com/43918312/146547471-44196405-d9e3-4847-9cd5-ca9a59e47832.PNG)


Now, we have all basic information to calculate of membership degress. Calculate each elevator degree one by one:

Elevator 1:

![el1_degree](https://user-images.githubusercontent.com/43918312/146547786-bd62799d-399f-4c6b-a3a7-c3f170d9b679.PNG)

Elevator 2:

![el2_degree](https://user-images.githubusercontent.com/43918312/146547821-875460dd-0839-4263-a856-69f628757222.PNG)

Elevator 3:

![el3_degree](https://user-images.githubusercontent.com/43918312/146547848-956dbee8-d28b-402c-ac08-06ca671bc57f.PNG)

We have everyting but the rules. Because of we have to create rules. But if we want to decrese waiting time with fuzzy logic, we have to calculate each elevator's. So, i create 11 different rules and we are going to use these rules for each elevator. We have 3 elevators that means we have 33 rules.

Elevator 1 rules:

![el1_rules](https://user-images.githubusercontent.com/43918312/146548520-cfd288db-8ecc-4ea3-8be3-043c38824bd5.PNG)

Elevator 2 rules:

![el2_rules](https://user-images.githubusercontent.com/43918312/146548566-24f516c2-843b-4f43-8a23-88efeffe95a8.png)

Elevator 3 rules:

![el3_rules](https://user-images.githubusercontent.com/43918312/146548591-eaf2ef2b-aa1c-4e00-a20e-a77dcb4f8b3a.PNG)

We have to calculate union sets now. Actually, this three steps are some but we are doing these for each elevators. We have "low" , "medium" and "high" priority sections. We are calculating these.

![union_sets](https://user-images.githubusercontent.com/43918312/146548921-b123d944-dedc-422c-8e01-e0357600ca7a.PNG)

Now we are at fuzzy logic last step : Defuzzification.

![defuzzification](https://user-images.githubusercontent.com/43918312/146549197-21c322ef-9255-4efb-9931-6440bcefc4b4.PNG)

And we finally have result and completed fuzzy logic steps. After that we take these outputs:

![result](https://user-images.githubusercontent.com/43918312/146549477-4277856b-1899-4583-9921-94c892563612.PNG)

Before this result there is some controls of elevator system. You can look code page.







