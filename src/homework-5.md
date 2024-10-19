# Homework 5

Ishan Pranav

October 12, 2024

Professor Divya Singhvi

OPMG 1 Operations Management

## Question 1

> Fix-Em-Up Industries restores classic cars. Their chairman wants to create a
> project network diagram to plan future restoration jobs. The following
> activities are required to restore a car. First, workers must disassemble the
> car and catalog the parts. Next, they must reupholster the seats, rechrome the
> bumpers, paint the body panels and rebuild the engine. Each of these
> activities may begin once the car has been disassembled and the parts have
> been cataloged. After the workers have finished rechroming the bumpers and
> painting the body panels, they can reassemble the body. After the seats are
> reupholstered and the body has been reassembled, they can install the
> reupholstered seats. After the engine is rebuilt and the body has been
> reassembled, the rebuilt engine can be installed. The list of activities is
> given below. Construct the network diagram for Fix-Em-Up Industries using the
> Activity-on-Arc method discussed in class.

| Activity | Description |
|:--------:|-------------|
| A | Disassemble car & catalog parts |
| B | Paint Body Panels |
| C | Rebuild Engine |
| D | Rechrome Bumpers |
| E | Reupholster seats |
| F | Reassemble body |
| G | Install reupholstered seats |
| H | Install rebuilt engine |

## Question 2

> NYC Real Estate is purchasing an old office building in order to renovate it.
> The renovation project consists of 7 activities which are given below. The
> duration of each activity is given in weeks and the precedence relationships
> among the activities are given as well.

| Activity | Description | Immediate predecessors | Duration (weeks) |
|----------|-------------|------------------------|------------------|
| A | Secure Financing | – | 3 |
| B | Hire Employees | – | 7 |
| C | Buy Materials | A | 5 |
| D | Purchase Property | A | 3 |
| E | Clean Old Building | D | 2 |
| F | Perform Renovation | B, C, E | 3 |
| G | Sign Tenants | D | 7 |

### Question 2 Part A

> Draw the precedence diagram for this project.

### Question 2 Part B

> Using the critical path method learned in class, determine the earliest start,
> earliest finish, latest start and latest finish times of each activity. In
> addition, compute the slack of each activity.

### Question 2 Part C

> What is the minimum amount of time needed to complete the renovation project?
> Also, what are the critical activities and the critical path(s) of the
> project?

### Question 2 Part D

> Suppose that due to market competition, NYC Real Estate would like to complete
> its renovation project within the next 9 weeks. For each week beyond the 9
> weeks deadline, it faces a $800 penalty. The following table details NYC Real
> Estate’s project crashing options.

| Activity | Immediate predecessors | Normal duration (weeks) | Crash duration (weeks) | Normal cost (\$) | Crash cost (\$) | Crash cost (\$/week) |
|:--------:|:----------------------:|:------------------------:|:-:|:-:|:-:|:-:|
| A | – | 3 | 2 | 1,300 | 2,150 | 850 |
| B | – | 7 | 5 | 800 | 1,700 | 450 |
| C | A | 5 | 5 | 2,000 | 2,000 | - |
| D | A | 3 | 1 | 1,600 | 2,200 | 300 |
| E | D | 2 | 1 | 1,500 | 1,750 | 250 |
| F | B, C, E | 3 | 1 | 1,000 | 2,000 | 500 |
| G | D | 7 | 3 | 2,200 | 3,800 | 400 |
