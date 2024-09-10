# Homework 1

Ishan Pranav

September 12, 2024

Professor Divya Singhvi

OPMG 1 Operations Management

## Definitions

Let $L$ be the inventory, $\lambda$ be the flow rate of inventory, and $w$ be the wait time.

Then, by Little's law, we have:

$$L=\lambda w.$$

## Question 1

> Draw a process flow diagram for your favorite coffee shop. List the relevant
> inputs, activities, and outputs in three columns.

## Question 2

> Suppose that 450 visitors enter a carnival every hour. The visitors spend 90
> minutes waiting in line for and going on the rides and then another 30 minutes
> eating. How many visitors are there at any given point in time at the
> carnival?

We can apply Little's law.

$$L=\lambda w,$$

$$L=\left(450\,\frac{\text{visitors}}{\text{h}}\right)(1.5\text{ h}+0.5\text{h}),$$

$$L=\left(\frac{450\text{ visitors}}{1\text{ h}}\right)(2\text{ h}),$$

$$L=900\text{ visitors}.$$

On average, there are 900 visitors at the carnival at any given time.

## Question 3

> At the doctor’s office there are 12 check-in machines and expect that a
> patient will spend 15 minutes checking in before proceeding to the main
> waiting room. If a patient will spend on average 20 minutes in the waiting
> room, what is the maximum number of seats that the doctor’s office should
> install in the waiting room?

We can apply Little's law for each process.

For the check-in process, let $L_1$ denote the maximum inventory, $\lambda_1$
denote the capacity, and $w_1$ denote the average wait time.

$$L_1=\lambda_1w_1,$$

$$12\text{ patients}=\lambda_1\cdot15\text{ min},$$

$$\lambda_1=\frac{12\text{ patients}}{15\text{ min}}.$$

For the waiting process, let $L_2$ denote the maximum inventory, $\lambda_2$
denote the capacity, and $w_2$ denote the average wait time. The capacity is
limited by the capacity of the check-in process; thus, $\lambda_1=\lambda_2$.

$$L_2=\lambda_1w_2,$$

$$L_2=\frac{12\text{ patients}}{15\text{ min}}\cdot 20\text{ min},$$

$$L_2=16\text{ patients}.$$

Thus, the doctor's office should install a maximum of 16 seats.
