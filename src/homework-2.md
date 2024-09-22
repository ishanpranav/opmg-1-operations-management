# Homework 2

Ishan Pranav

September 24, 2024

Professor Divya Singhvi

OPMG 1 Operations Management

## Question 1

> Suppose that loading a tray of cookies into the oven takes Kristen’s roommate
> 4 minutes instead of 1 minute as in the case discussed in class. What is the
> minimum amount of time that it will take Kristen and her roommate to fill a
> rush order of 2 dozen cookies? Use a Gantt chart to find your answer.

## Question 2

> Suppose that Tom, Abby, and Issac are working at a furniture workshop. The
> furniture-making process consists of four activities: cutting the wood,
> assembling the frame, adding the cushion, and adding finishing touches. Tom
> cuts the wood, Abby handles the frame assembly and finishing, and Issac is
> adding the cushion. The process flow diagram is shown below.

![Process flow diagram](../images/homework-2-2.png "Process flow diagram for a furniture workshop")

### Question 2 Part A

> Calculate the capacity of each resource.

Let $t$ represent the cycle time and $\lambda$ represent the capacity.

- __Cutting wood:__ We have $t=8~\frac{\text{min}}{\text{piece}}$. Then $\lambda=\frac{1}{t}=\frac{1\text{ piece}}{8\text{ min}}\cdot\frac{60\text{ min}}{1\text{ h}}=7.5~\frac{\text{pieces}}{\text{h}}$.
- __Assembling frame:__ We have $t=6~\frac{\text{min}}{\text{piece}}$. Then $\lambda=\frac{1}{t}=\frac{1\text{ piece}}{6\text{ min}}\cdot\frac{60\text{ min}}{1\text{ h}}=10~\frac{\text{pieces}}{\text{h}}$.
- __Adding cushion:__ Similarly, $\lambda=10~\frac{\text{pieces}}{\text{h}}.$
- __Adding finishing touches:__ We have $t=4~\frac{\text{min}}{\text{piece}}$. Then $\lambda=\frac{1}{t}=\frac{1\text{ piece}}{4\text{ min}}\cdot\frac{60\text{ min}}{1\text{ h}}=15~\frac{\text{pieces}}{\text{h}}$.

### Question 2 Part B

> What is the bottleneck of the process and what is the capacity of the process?

The bottleneck of the process is the "cutting wood" resource, since it has the
lowest capacity. Since the capacity of the process is limited by its bottleneck,
the capacity of the process is $\lambda^*=7.5~\frac{\text{pieces}}{\text{h}}$.

### Question 2 Part C

> Calculate the utilization of each resource assuming that the process is
> operating at maximum capacity.

Let $\rho$ represent the utilization.

- __Cutting wood:__ Since "cutting wood" is the bottleneck process, it has $\rho=100\%$.
- __Assembling frame:__ We have $\rho=t\lambda^*=8~\frac{\text{min}}{\text{piece}}\cdot 7.5~\frac{\text{pieces}}{\text{h}}=45~\frac{\text{min}}{\text{h}}=75\%$.
- __Adding cushion:__ Similarly, we have $\rho=75\%$.
- __Adding finishing touches:__ We have $\rho=t\lambda^*=4~\frac{\text{min}}{\text{piece}}\cdot 7.5~\frac{\text{pieces}}{\text{h}}=30~\frac{\text{min}}{\text{h}}=50\%$.

### Question 2 Part D

> Suppose that Tom is paid $18 per hour but only for the amount of time that he
> actually works, that Abby is paid $20 per hour but only for the amount of time
> that she actually works and that Issac is paid $16 per hour but also only for
> the amount of time that he actually works. Suppose also that each furniture
> piece sold brings a revenue of $140 and has raw materials cost of $80.
> Assuming that the furniture factory is operating at its maximum capacity, what
> is the profit per hour after paying Tom, Abby and Issac their salaries?

| Income statement | $ per hour |
|---|-----------:|
| __Revenues__ | __1,050__ |
| Raw materials expense | | 600 |
| Direct labor expense - Tom | 18 |
| Direct labor expense - Abby | 15 |
| Direct labor expense - Issac | 8 |
| __Cost of goods sold__ | __641__ |
| __Gross profit__ | __409__ |

The gross profit is $409 per hour.
