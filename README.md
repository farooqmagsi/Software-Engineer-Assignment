
Title And Authors:-

Automated Repair of Feature Interaction Failures in Automated Driving Systems

•	Raja Ben Abdessalem

•	Annibale Panichella

•	Shiva Nejati

•	Conference Program ISST-2020

Introduction And Motivation:-

Software for automated driving systems in Short form (ADS) is often composed of several units of functionality, known as ADS features, that automate specific driving tasks example automated emergency braking, automated traffic sign recognition, and automated cruise control. Using this information, ADS features independently determine the car maneuver for the next time step. Some maneuvers issued by different features may be conflicting. For example, automated cruise control may order the ego car to accelerate to follow th Integration rules are likely to be erroneous, leading to system safety requirements violations. In particular, we identify two general ways where the integration rules may be wrong: (1) The preconditions of the rules may be wrong e speed of the leading car while, at the same time, the automated traffic sign recognition feature orders the ego car to stop since the car is approaching an intersection with a traffic light that is about to turn red. They are typically defined manually by engineers based on their domain knowledge and are expected to ensure safe and desired car maneuvering. Automated driving systems use integration rules to resolve conflicts among multiple maneuvers issued by different ADS features. The rules determine what feature output should be prioritized at each time step based on the environment factors and the current state of the system.

Research And Methodology:-

Research Question No.1:- How effective is ARIEL in repairing integration faults? We assess the effectiveness of ARIEL by applying it to industrial ADS systems with faulty integration rules.
Research Question No.2:- How does ARIEL compare to baseline program repair approaches? In this research question, we compare ARIEL with three baselines that we refer to as Random Search (RS), Random Search with Multiple Mutations (RS-MM) and Genetic Programming (GP). We compare ARIEL with the baselines by evaluating their effectiveness (the ability to repair faults) and efficiency (the time it takes to repair faults).
We describe our baseline methods: Random Search with Multiple Mutation and Genetic Programming and the parameters used in our experiments. Random Search. RS is a natural baseline to compare with because prior work  showed that it is particularly effective in the context of program repair, often outperforming evolutionary algorithms. RS does not evolve candidate patches but generates random patches by mutating the original rules only once using either the modify or shift operator. The final solution patch among all randomly generated patches is the one with the best baseline value. Random Search with Multiple Mutations . RS-MM is an improved variant of RS where multiple mutations are applied to the faulty rule set rather than one single mutation as done in RS. In other words, RS-MM generates random patches using the same operator applied in ARIEL Algorithm 2. Thus, with the second baseline, we aim to assess whether the differences if any between random search and ARIEL are due to the mutation operator or the evolutionary search we proposed in this paper.


Result:- 

Answer Research Question.no1:-  We apply ARIEL 20 times to AutoDrive1 and AutoDrive2 until a patch is found that passes all the test cases given as input. For both case study systems and for all the runs, ARIEL was able to repair the integration rules in the underlying ADS and terminate successfully. The box-plots in show the time needed for ARIEL to repair the integration rules of AutoDrive1 and AutoDrive2, respectively, over 20 independent runs. As shown in the figures, ARIEL is able to repair all the integration faults in less than nine hours for AutoDrive1 and in less than 16 hours for AutoDrive2. The average repair time for AutoDrive1 and AutoDrive2 is five hours and 11 hours, respectively. We note that failures in AutoDrive1-2 were caused by independent faults in different parts of the code. Recall from Section 3.2 that in order to resolve failures, ARIEL fixes the following fault types in the integration rules: (I) wrong operator/threshold, (II) wrong rule ordering and (III) a combination of both (I) and (II). For AutoDrive1, three faults were of type (I) and one was of type (III). For AutoDrive2, both faults were of type (II).
Answer Research Question.no2:- We ran ARIEL, GP, RS-MM and RS 20 times for 16 hours. We selected a 16 hour timeout since it was the maximum time required by ARIEL to find patches for both AutoDrive1 and AutoDrive2. Also, recall that we had four failing test cases for AutoDrive1 and two failing test cases for AutoDrive2. The number of failing test cases in AutoDrive1 and AutoDrive2 that are left unresolved over time by different runs of ARIEL, GP, RS-MM and RS. We show the results at every two-hour interval from 0 to 16h. all 20 runs of ARIEL are able to solve all the failing test cases in AutoDrive1 after nine hours and in AutoDrive2 after 16 hours. Note that this is consistent with the result. Table 2 reports the number of runs of GP, RS-MM, and RS, out of 20 runs, that resolved failures in AutoDrive1 and in AutoDrive2. As the above results show, GP had the worst performance in repairing the integration rules. This is because GP is a populationbased search algorithm that evolves a pool of candidate patches iteratively. As a result, none of the GP runs could perform more than two iterations, hence its poor performance.

Conclusion:-

We proposed a repair technique to automatically resolve integration faults in automated driving systems (ADS). Our approach localizes faults over several lines of code to fix complex integration faults and deals with the scalability issues of testing and repairing ADS. The results indicate that our repair strategy can fix the integration faults in these two systems and outperforms existing automated repair techniques. Feedback from domain experts indicates that the patches generated by our approach are understandable by engineers and could not have been developed by them without any automation assistance.
