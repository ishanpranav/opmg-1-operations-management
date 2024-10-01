# Homework 3

Ishan Pranav

October 1, 2024

Professor Divya Singhvi

OPMG 1 Operations Management

## Definitions

__Exponential distribution.__

Let $X$ represent an exponentially-distributed random variable with rate
parameter $\lambda_X$. Then for all values $x$ of $X$, we have
$P(X\leq x)=F(x;\lambda)$, where

$$F(x;\lambda_X)=
\begin{cases}
1-e^{-\lambda_Xx},&x\geq 0;\\
0,&x<0.
\end{cases}$$

__M/M/S system.__

Let $S$ denote an multiple-server system (M/M/S) with a single queue $Q$. Let
$W_S$ denote the average wait time in $S$, let $W_Q$ denote the average wait
time in $Q$, and let $L_S$ denote the average number of units in $S$. Let
$\lambda$ denote the arrival rate and $\mu$ denote the service rate. Then:

$$W_Q=\frac{L_Q}{\lambda}.$$

$$W_S=W_Q+\frac{1}{\mu}.$$

$$L_S=\lambda W_S.$$

## Introduction

> Customers arrive at the checkout area of New Navy with the inter-arrival time
> being exponentially distributed at a rate of 100 customers per hour. At the
> checkout area, the service time of each customer is exponentially distributed,
> and on average each cashier can serve 20 customers per hour. The store has
> hired 8 cashiers to checkout customers and the checkout area consists of a
> single pool of cashiers with one common line in front of them.

## Part A

> What is the probability that a customer’s service time is less than 6 minutes?

Let $X$ denote the customer's service time. We know $X$ is an
exponentially-distributed random variable with a rate of
$\lambda_X=20~\frac{\text{customers}}{\text{h}}$.

$$\lambda_X=\frac{20\text{ customers}}{1\text{ h}}\cdot\frac{1\text{ h}}{60\text{ min}}=\frac{1}{3}~\frac{\text{customers}}{\text{min}}.$$

$$\begin{align*}
P\left(X<6~\frac{\text{min}}{\text{customer}}\right)&=P\left(X\leq 6~\frac{\text{min}}{\text{customer}}\right)-P\left(X=6~\frac{\text{min}}{\text{customer}}\right)\\
&=F\left(6~\frac{\text{min}}{\text{customer}};\lambda_X\right)-0\\
&=F\left(6~\frac{\text{min}}{\text{customer}};\frac{1}{3}~\frac{\text{customers}}{\text{min}}\right)\\
&=1-\exp\left(-\frac{1}{3}~\frac{\text{customers}}{\text{min}}\cdot 6~\frac{\text{min}}{\text{customer}}\right)\\
&=1-\exp(-2)\\
&\approx 86.4664\dots\%.
\end{align*}$$

The probability that a customer's service time is less than 6 minutes is about
86.47%.

## Part B

> What is the average number of customers waiting in the queue to be checked
> out? This does not include the customers being checked out.

Let $Q$ denote the queue and $L_Q$ denote its average length. The average
arrival rate is $\lambda=100~\frac{\text{customers}}{\text{h}}$ and the average
service rate is $\mu=20~\frac{\text{customers}}{\text{h}}$.
Then $\frac{\lambda}{\mu}=\frac{100}{20}=5$ and the number of service channels
$s=8$ (cashiers). Using precomputed values of $L_Q$, we have $L_Q\approx 0.279\dots$
(customers).

The average number of customers waiting in the queue to be checked out is about
0.28.

## Part C

> What is the average service time?

Since service time is exponentially distributed with rate parameter $\mu$, the
average service time is
$\frac{1}{\mu}=\frac{1}{20~\frac{\text{customers}}{\text{h}}}=0.05~\frac{\text{h}}{\text{customer}}=12~\frac{\text{min}}{\text{customer}}$.

The average service time is 12 minutes per customer.

## Part D

> What is the average total number of customers in the checkout area? This
> includes the customers who are waiting to be checked out and the customers
> being checked out.

Let $S$ denote the checkout area and $Q$ be its queue. Let $L_S$ denote the
number of customers in $S$ and $W_S$ denote the average wait time in $S$.

Of course,

$$L_S=\lambda W_S.$$

$$W_S=\frac{L_Q}{\lambda}+\frac{1}{\mu}.$$

Therefore,

$$L_S=\lambda\left(\frac{L_Q}{\lambda}+\frac{1}{\mu}\right).$$

Intuitively,

$$L_S=L_Q+\lambda\cdot\frac{1}{\mu}.$$

From Part B, we have $L_Q\approx 0.279\dots$, and from Part C, we have
$\frac{1}{\mu}=12~\frac{\text{min}}{\text{customer}}$.

$$L_S\approx(0.279\dots)+\frac{100\text{ customers}}{60\text{ min}}\cdot12~\frac{\text{min}}{\text{customer}}\approx 20.279\dots\text{ customers}.$$

The average total number of customers in the checkout area is about 20.28.
