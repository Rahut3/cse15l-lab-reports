# Lab Report 5


In this final lab report I am writing about a debugging scenario between a student and a TA.



## Part One

**Students question:**

![image](https://github.com/Rahut3/cse15l-lab-reports/assets/116214329/e849ec00-c8a0-4d99-8e22-ca68d8969aeb)

*Attached files*

![image](https://github.com/Rahut3/cse15l-lab-reports/assets/116214329/0ebbf242-3156-4378-9c59-dbcba6f154bb)

![image](https://github.com/Rahut3/cse15l-lab-reports/assets/116214329/3edb8f29-6350-4772-a52c-dcf57f59daa0)

![image](https://github.com/Rahut3/cse15l-lab-reports/assets/116214329/9883ecbd-d3d9-400d-af0f-91ae0296d692)



**TA's response**

Hi, Rahut looks like the error is being caused from the grade.sh file. The error is caused by you not including the hamcrest class path in your bash script when running javac and java. Therefore the bash script couldn't find the hamcrest path so therefore it wouldn't excute the JUNIT test. To fix this make sure you include the hamcrest class path inside your javac/java statements. Take a look at Week 3 to see the proper command to run JUNIT tests.


**Student Response**

Thank you! This is the changes I made to my bash script to make it run the JUNIT tests.

*Fixed grade.sh:*

```
javac -cp .:lib/junit-4.13.2.jar:lib/hamcrest-core-1.3.jar test.java


if [ $? -eq 0 ]; 
then
    echo "Compile successful."

    java -cp .:lib/junit-4.13.2.jar:lib/hamcrest-core-1.3.jar org.junit.runner.JUnitCore test

else
    echo "Compile failed."
fi
```

*Output:*

![image](https://github.com/Rahut3/cse15l-lab-reports/assets/116214329/6c95c0a5-1710-4d94-b196-c88bd26d2980)
