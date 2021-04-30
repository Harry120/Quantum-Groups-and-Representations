# Quantum Mechanics, Groups and Representations

Quantum mechanics models a physical system with a Hilbert space $\H$. For example, $L^2(\R^3, \C)$ is often used to model a single particle in $\R^3$. Explicitly, this means that at any given time, we associate the state of the particle with a vector $\ket{\phi(t)} \in L^2(\R^3, \C)$. We think of this as representing the 'distribution' of the particle in space - the value of $\ket{\phi(t)}$ at a point $\vec{x}$ is supposed to represent the probability density of finding the particle around $\vec{x}$. 

Of course, we can also work with a finite dimensional Hilbert space $\C^n$. The physical interpretation of states in this situation is less immediate - in fact, such a Hilbert space is used to represent the 'internal properties' of the particle. 

In the quantum formalism, any observable quantity is associated with a hermitian operator on $\H$. Surprisingly, it turns out that most of the interesting observable quantities can be deduced from the symmetries of $\H$ itself (a symmetry is a transformation that leaves the inner product of $\H$ invariant - i.e. a symmetry is a unitary action). Briefly, the reason for this is as follows:
\begin{enumerate}
    \item Suppose $G$ is a Lie group that has a unitary representation $\pi$ on $\H$. The tangent space at the identity $e \in G$ is a vector space that can be made into a lie algebra $\g$. 
    \item The derivative of $\pi$ at the identity in $G$ gives a unitary lie algebra representation $\pi' : \g \to \mathfrak{u}(\H)$. 
    \item Elements of $\mathfrak{u}(\H)$ are skew adjoint, so for any $X \in \g$, a hermitian operator $O = i\pi'(X)$ can be defined, and this will be an observable of the quantum system. 
\end{enumerate}

The purpose of this report is to explore representation theory and then examine this connection with quantum mechanics. To begin with, we look at the representations of finite groups. Although quantum mechanics is more concerned with the representations of infinite groups (particularly Lie groups), this serves as a starting point to introduce the main themes of representation theory. In contrast, the section on Lie theory does not dive much deeper than the definitions of essential concepts, and instead spends more time working through several examples that will be important for the section on quantum mechanics. 

The section on Quantum mechanics begins with an overview of the core concepts and a brief discussion of some philosophical interpretations. We then explore two examples of situations where the irreducible representations of a Lie group generate a set of observables. In particular, we explore how orbital angular momentum operators arise from the action of $SO(3)$ on $L^2(\R^3, \C)$, and how spin angular momentum operators arise from the action of $SU(2)$ on $\C^n$.
