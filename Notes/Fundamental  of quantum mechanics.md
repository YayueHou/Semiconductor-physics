---
export_on_save:
    puppeteer: true # export PDF on save
---
```
1952033 侯雅玥 2020.10.7
```
# QUANTUM MECHANIC
## Wave Function

* Schrodinger function
$$ i\hbar \frac{\partial {\Psi}}{\partial t}=-\frac{\hbar^2}{2m}\frac{\partial^2{\Psi}}{\partial x^2}+ {V\Psi} $$
* Actually, $  V $is called potential function and is     independent of time $t$ and it reference to the potential energy of particle 
  ***
  According to the definition of potential function
$$   \boldsymbol{E}=-\nabla \varphi(\boldsymbol{r})$$
 $  \boldsymbol E$ is a electrical field function
  ***
* hence Schrodinger function can be discribe as 
$$  {\Psi}= {\psi (x) \phi(t)} $$
$ {\psi (x) }$is the position-dependent portion of wave function and $ {\phi(t)} $ is the time-dependent portion of wave function.
* hence ,we can write the wave function as 
$$ i\hbar \frac{\partial ( {\psi (x) \phi(t)) }}{\partial t}=-\frac{\hbar^2}{2m}\frac{\partial^2( {\psi (x) \phi(t)}) }{\partial x^2}+ {\psi (x) \phi(t)V(x)} $$
$$ i\hbar {\psi(x)} \frac{\partial   {\phi(t) }}{\partial t}=-\frac{\hbar^2}{2m} {\phi(t)}\frac{ \partial^2 {\psi (x)} }{\partial x^2}+ {\psi (x) \phi(t)V(x)}$$
$$ i\hbar\frac{\partial   {\phi(t) }}{ {\phi(t)}\partial t}=-\frac{\hbar^2}{2m}\frac{ \partial^2 {\psi (x)} }{ {\psi(x)}\partial x^2}+  {V(x)}$$

* For the left portion of the function is only related to $t$ and the right portion is only related to $x$ , hence both two parts are constant. Denote this constant by $\eta $ ,then
$$ \eta=i\hbar\frac{\partial   {\phi(t) }}{ {\phi(t)}\partial t}=-\frac{\hbar^2}{2m}\frac{ \partial^2 {\psi (x)} }{ {\psi(x)}\partial x^2}+  {V(x)}$$
$$  {\phi(t)}=Ce^{-j\frac{\eta t}{\hbar}}$$
And according to eular therom we can get ,
$$  {\phi(t)}=C(cos(\frac{\eta t}{\hbar})-jsin(\frac{\eta t}{\hbar}))$$
It's a sinusoidal wave, with $\omega=\frac{\eta}{\hbar}$ ,then we can get ,
$$ T=\frac{2\pi}{\omega}=\frac{2\pi\hbar}{\eta}=\frac{h}{\eta}$$
$$ \nu=\frac{1}{T}=\frac{\eta}{h}$$
$$ \eta=h\nu=E$$
$\eta$ refrence to the energy of the sinusoidal wave.
* hence ,
$$ E=\eta=-\frac{\hbar^2}{2m}\frac{ \partial^2 {\psi (x)}}{ {\psi(x)}\partial x^2}+  {V(x)}$$
$$ \frac{2m}{\hbar^2}(E-  {V(x)}) {\psi(x)}+\frac{ \partial^2 {\psi (x)} }{\partial x^2}=0$$

## Physical Meaning of Wave Function
* $| {\Psi(x,t)}|^2$ refers to the probability density of finding the particle.
$$ {\phi(t)}=Ce^{-j\omega t}$$
$$ | {\Psi(x,t)}|^2= {\Psi\Psi^*}= {|\psi(x)|^2}Ce^{-j\omega t}Ce^{j\omega t}=C^2 {|\psi(x)|^2}$$
We can incorporate $C$ into ${\psi(x)}$ , then
$$ |{\Psi(x,t)}|^2= {|\psi(x)|^2}$$
## Boundry Conditions
* The function need to be normalized , for it is a discription of probability density , hence 
$$  \int_{-\infty}^\infty  {|\psi(x)|}^2dx=1$$
* If the energy $E$ and the ${V(X)}$ is both finite ,then there will be two boundry conditons:
   1. ${\psi(x)}$ must be finite , single-valued , continous
   2. $\frac{\partial {\psi(x)}}{\partial x}$ must be finite , single-valued , continous
## Application of Wave Function
###   Electrons in free space
* When there is no force acting on the particle , so $V(x)$ must be a constant .
* ***
we have
        $$ E=h\nu =E_k+V(x)$$
        $$ E_k=\frac{h^2}{2m}$$
        $$ E-V(x)=\frac{h^2}{2m}$$
***
* $E_k\geq 0$ in free space , hence $E\geq V(x)$
Assume $V(x)=0$ ,
$$ \frac{2m}{\hbar^2}E {\psi(x)}+\frac{ \partial^2 {\psi (x)} }{\partial x^2}=0$$
***
 The solution of linear differential equation with constant coefficients of the second order is as follows :

 if the characteristic function has
 1. 2 different real root
  $$ y=C_1e^{y_1x}+C_2e^{y_2x}$$
 2. 2 same real root
  $$ y=(C_1+C_2x)e^{y_1x}$$
 3. 2 conjugate complex root
  $$ y=e^{\alpha x}(C_1cos(\beta x)+C_2sin(\beta x))$$
  $$ y_1=e^{\alpha x}cos(\beta x) \qquad y_2=e^{\alpha x}sin(\beta x)$$
***
* hence ,  the solution of the partial differential equation is :
$$ \psi(x)=C_1exp[\frac{\sqrt{2mE}}{\hbar}ix]+C_2exp[-\frac{\sqrt{2mE}}{\hbar}ix] $$ 
Assume,
$$k=\frac{\sqrt{2mE}}{\hbar}$$
then ,
$$ \psi(x)=C_1exp[ikx]+C_2exp[-ikx] $$ 
* hence , recall the time-dependent function $\phi(t)$ ,  there is
$$ \Psi(x,t)=exp[-jwt] (C_1exp[ikx]+C_2exp[-ikx])$$
We can assume that the particle motion direction is +x then there is $C_2=0$
* The relationship between $k$ and $\lambda$ can be derived as follows :
  $$ k=\frac{\sqrt{2mE}}{\hbar}$$
  And because $V(x)=0$  , hence $E=\frac{1}{2}mv^2$
  $$ E=\frac{1}{2}mv^2=\frac{p^2}{2m} $$
  $$ k=\frac{p}{\hbar}$$
And according to
 $$p=\frac{h}{\lambda} $$
 $$ k=\frac{2\pi}{\lambda} $$
 And ultimately , we get the result of $\Psi$
 $$ \Psi(x)=C_1exp[j(kx-\omega t)] $$
$$\Psi\Psi^*=C_1C_1^*$$
$\Psi\Psi^*$is independent to positio , when the particle's  momentum is well-defined
###   The Infinite potential well
* In infinite potential well , there is 
$$V(\boldsymbol{x})=\begin{cases}\quad 0\qquad 0<r<a \\ \quad \infty \qquad x>a\quad  x<0    \end{cases} $$
When $x>a \qquad x<0$ , if E is finite then , $\psi(x)=0$ 
When $0<x<a$ , there is 
$$ \frac{2m}{\hbar^2}E {\psi(x)}+\frac{ \partial^2 {\psi (x)} }{\partial x^2}=0$$
we define :
$$\frac{2mE}{\hbar^2}=k^2\qquad k=\frac{\sqrt{2mE}}{\hbar}$$
the solution is like :
$$ \psi(x)=Asin(kx)+Bcos(kx)$$
* According  to boundry condition , when $x=a$ and $x=0$ , $\psi(x)=0$
hence $B=0$ and $Asin(ka)=0$ , hence $ka=n\pi$. 
For $k\neq 0 \quad a\neq 0$ , $kx\neq 0$ , hence $n\pi\neq 0 \quad n\neq 0$
And when $n<0$ , for $Asin(-n\pi)=-Asin(n\pi)$ the negative ones can be conbined into $A$
$$ \psi(x)=Asin(kx)=Asin(\frac{n\pi}{a}x) \quad(n=1,2,3,...)$$
Normalization :
$$ |{\Psi(x,t)}|^2= {|\psi(x)|^2}$$
$$\int_{-\infty}^{+\infty}|{\Psi(x,t)}|^2=\int_{-\infty}^{+\infty}{|\psi(x)|^2}=\int_{0}^{a}A^2sin^2(\frac{n\pi}{a}x)=\frac{aA^2}{2}=1$$
hence ,
$$ A=\sqrt{\frac{2}{a}}$$
$$\psi(x)=\sqrt{\frac{2}{a}}sin(\frac{n\pi}{a}x)\quad(n=1,2,3,...)$$
###   The Step potential function
* The potential function is :
  $$ V(x)=\begin{cases} 0\quad x<0 \\ V_0 \quad x>0  \end{cases} $$
  
* The incident flux and reflected flux are neither 0 , 
* hence in the region $x<0$
$$ \frac{2m}{\hbar^2}E {\psi(x)}+\frac{ \partial^2 {\psi (x)} }{\partial x^2}=0$$
the solution is like :
$$\psi_1(x)=A_1e^{ik_1x}+ B_1e^{-ik_1x}$$
And $k_1=\frac{\sqrt{2mE}}{\hbar}$
* The first term is a  traveling wave in direction of $+x$
The second term is a  traveling wave in direction of $-x$
So , the  first term refers to incident wave and the second term refers to the reflect wave.
* In th region of $x>0$ , $V(x)\neq 0$  , Assume $ V(x)>E$ , then
$$ \frac{2m}{\hbar^2}(E-  {V(x)}) {\psi(x)}+\frac{ \partial^2 {\psi (x)} }{\partial x^2}=0$$
$$ \frac{2m}{\hbar^2}(  {V(x)}-E) {\psi(x)}=\frac{ \partial^2 {\psi (x)} }{\partial x^2}$$
$$ k_2=\frac{\sqrt{2m(V(x)-E)}}{\hbar} $$
$$ V(x)=V_0\qquad k_2=\frac{\sqrt{2m(V_0-E)}}{\hbar}$$
Then there will be :
$$\psi_2(x)=A_2e^{k_2x}+ B_2e^{-k_2x}$$
According to the boundry condition of finite $A_2=0$
$$\psi_2(x)=B_2e^{-k_2x}$$
According to the boundry condition 
$$\psi_1(0)=\psi_2(0)=A_1+B_1=B_2$$
According to my comprehention , the variation of perticle at the two sides of $x=0$ is equal then ,
$$\frac{\partial{\psi_1(0)}}{\partial{x}}=\frac{\partial{\psi_2(0)}}{\partial{x}}$$
$$ ik_1A_1-ik_1B_1= -B_2k_2$$
Then there will be :
$$ B_1=\frac{ik_1+k_2}{ik_1-k_2}A_1 $$
$$ B_2=\frac{2ik_1}{ik_1-k_2}A_1 $$
