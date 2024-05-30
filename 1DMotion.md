---
layout: page
menu: yes
title: 1D Motion
---

# One Dimensional Motion

## TLDR

$$ a(t) = a $$

$$ v(t) = at + v_0 $$

$$ x(t) = \frac{1}{2}at^2 + v_0t + x_0 $$

## Introduction

We will use the following setup as our basis for understanding the simple motion of an object in one dimension:

![Ball sitting at 0 on x-axis](./figures/still_ball.jpg)

The ball at the center can roll in either the $+x$ or the $-x$ direction. Lets see how we can describe this motion. First, we will define the position of the ball, $x$, as a function of time, $t$. For a stationary ball:

$$ \vec{x}(t) = \vec{x}_0 $$

where $x_0$ is some arbitrary value. In our figure, $x_0=0$ because the ball is at $x=0$. We change $x$ to $\vec{x}$ because it is a vector. That is, it has both a magnitude and direction. Its magnitude is the distance from the origin, and its direction will be positive or negative.

## Velocity

This equation is not very useful because it tells us nothing about how the ball might move. Lets now say that the ball is moving at a constant _speed_ in the $x$ _direction_. We call this new vector velocity and denote it as a $\vec{v}$. Because $\vec{v}$ is constant, we can write a similar equation to our constant position:

$$ \vec{v}(t) = \vec{v}_0 $$

Now that the ball is moving, the position is no longer constant. There are two ways to think about how position might change.

### Dimensional Analysis

This is the simplest of the two methods. We know that velocity is how position changes over time, so we give it a unit of meters per second, or $\frac{m}{s}$. You might be more familiar with a velocity unit of miles or kilometers per hour. You can convert $m/s$ to these units. We know that position has a unit of meters. So, to get from velocity to position, it follows that we multiply by time to just get distance. Now our velocity equation looks like this:

$$ \vec{x}(t) = \vec{v}t + \vec{x_0} $$

We add $x_0$ because our $\vec{v}t$ term only gives us how position changes, not the final position. To get that, we need to know where the object started.

### Calculus

If you know calculus, this is an easier method of finding equations of motion. If velocity is how the position changes over time, then we can say that:

$$ \frac{d\vec{x}}{dt} = \vec{v}(t) $$

So, by integrating $\vec{v}$ with respect to $t$, we should arrive at our position equation.

$$ \vec{x}(t) = \int\vec{v}(t)dt $$

And by still following Equation 2 where velocity is constant, this is a relatively simple integral that gives us:

$$ \vec{x}(t) = \vec{v}t + \vec{x}_0 $$

### Velocity vs. Position

add figure with v vs t and x vs t

## Acceleration

Just as we said position can change over time, so can velocity. We call this acceleration. When you press the gas pedal on your car, you are increasing the speed you are traveling at, and therefore accelerating the car. Acceleration has units of meters per second, per second, or $\frac{m}{s^2}$.
For now, we will always assume a constant acceleration.

$$ \vec{a}(t) = \vec{a}_0 $$

Similar to how adding a velocity changes position, adding an acceleration changes our velocity equation. We can use a similar method of dimensional analysis, or say that acceleration is the derivative of velocity to find that $\vec{v}$ is now:

$$ \vec{v}(t) = \vec{a}t + \vec{v}_0 $$

To find our position equations with an acceleration present we can integrate acceleration twice. There are methods of deriving this equation without calculus, however they are much more tedious.

$$ \vec{x}(t) = \int\int\vec{a}(t)dt = \int(\vec{a}_0t + \vec{v}_0)dt = \frac{1}{2}\vec{a}t^2 + \vec{v}_0t + \vec{x}_0 $$