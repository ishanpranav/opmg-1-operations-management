# Homework 4

Ishan Pranav

October 12, 2024

Professor Divya Singhvi

OPMG 1 Operations Management

## Question 1

> A tech company, Innovatech, manufactures two types of electronic devices:
> smartphones and tablets. Each smartphone is sold for $500 and each tablet is
> sold for $350. The production of these devices requires time on two different
> machines. Each smartphone requires 4 hours on Machine X and 2 hours on Machine
> Y, while each tablet requires 3 hours on Machine X and 3 hours on Machine Y.
> After being produced, the devices are tested, which takes 1.5 hours per
> smartphone and 2 hours per tablet. Machine X is available for 120 hours per
> week, and Machine Y for 100 hours per week. There are 80 hours available per
> week for testing. The marketing department estimates a maximum demand of 30
> smartphones and 50 tablets per week.

> To determine how many smartphones and tablets to produce, the CEO of
> Innovatech has set up the following linear program.

> Find the optimal number of smartphones and tablets to manufacture and the
> optimal profit by solving the linear program using both the enumerating corner
> points method and the isoprofit line method. Also, identify the binding and
> non-binding constraints and the slack of each constraint. Assume fractional
> production of smartphones and tablets is possible.

Maxmize:

$$f(x_1,x_2)=500x_1+350x_2.$$

Subject to:

$$4x_1+3x_2\leq 120,$$
$$2x_1+3x_2\leq 100,$$
$$1.5x_1+2x_2\leq 80,$$
$$x_1\leq 30,$$
$$x_1\geq 0,$$
$$x_2\geq 0.$$

The optimal allocation is $(x_1=30,x_2=0)$, or 30 smartphones and no tablets.
Thus the optimal profit in dollars is
$f(x_1,x_2)=(500\times 30)+(350\times 0)=15000$, or \$15,000.00.

We can demonstrate this result using two methods.

__Corner-points method.__

Analyzing the corner points, clockwise:

| $x_1$ | $x_2$ | $f(x_1,x_2)$ | Profit ($) |
|:-----:|:-----:|-----|-----------:|
| $0$ | $33.\overline{3}$ | $(500\times 0)+(350\times 33.\overline{3})$ | 11,666.66 |
| $10$ | $26.\overline{6}$ | $(500\times 10)+(350\times 26.\overline{6})$ | 14,333.33 |
| $30$ | $0$ | $(500\times 30)+(350\times 0)$ | 15,000.00 |
| $0$ | $0$ | $(0\times 0)+(0\times 0)$ | 0.00 |

We have the optimal allocation $(x_1=30,x_2=0)$ with $f(x_1,x_2)=15000$.

__Isoprofit lines method.__

Since the objective function is of the form $f(x_1,x_2)=a_1x_1+a_2x_2$, its
slope is of the form $-\frac{a_1}{a_2}$. For $f(x_1,x_2)=500x_1+350x_2$, the
slope of the objective function is $-\frac{500}{350}=-\frac{10}{7}$. Therefore,
the slope of the isoprofit line is $-\frac{10}{7}$.

Graphically, the isoprofit line with slope $-\frac{10}{7}$ that is tangent to a
corner point iis $15000=500x_1+350x_2$. Thus $f$ is maximized when
$f(x_1,x_2)=15000$. The point of tangency is $(x_1=30,x_2=0)$, so this is the
optimal allocation and \$15,000 is the maximum profit.

Using the optimal solution, we can classify the constraints.

__Constraint classification.__

| Expression | Constraint | Evaluation | Optimum | Type | Slack |
|------------|------------|------------|:-------:|:----:|:-----:|
| $4x_1+3x_2$ | $\leq 120$ | $(4\times 30)+(3\times 0)$ | $120$ | Binding | $0$ |
| $2x_1+3x_2$ | $\leq 100$ | $(2\times 30)+(3\times 0)$ | $100$ | Binding | $0$ |
| $1.5x_1+2x_2$ | $\leq 80$ | $(1.5\times 30)+(2\times 0)$ | $45$ | Non-binding | $35$ |
| $x_1$ | $\leq 30$ | $30$ | $30$ | Binding | $0$ |
| $x_1$ | $\geq 0$ | $30$ | $30$ | Non-binding | $30$ |
| $x_2$ | $\geq 0$ | $0$ | $0$ | Binding | $0$ |

## Question 2
