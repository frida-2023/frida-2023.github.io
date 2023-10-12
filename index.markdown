---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

# The 10th Workshop on Formal Reasoning in Distributed Algorithms

Date: Monday October 9th, 2023
Location: L'Aquila, Italy

The workshop is organized as part of [DISC 023](http://www.disc-conference.org).

## Confirmed Speakers

* [Karine Altisen](https://www-verimag.imag.fr/Karine-Altisen-102), University of Grenoble & Verimag
* [Hagit Attiya](https://hagit.net.technion.ac.il/), Technion
* [Manuel Bravo](https://angbrav.github.io/), Informal Systems
* [Ali Ebnenasir](https://www.mtu.edu/cs/department/people/faculty/ebnenasir/), Michigan Technological University
* [Pierre Fraigniaud](https://www.irif.fr/users/pierref/index), CNRS & IRIF
* [Alexey Gotsman](https://software.imdea.org/~gotsman/), IMDEA Software Institute
* [Rotem Oshman](https://www.cs.tau.ac.il/~roshman/), Tel Aviv University
* [Louis Penet de Monterno](https://www.lix.polytechnique.fr/member/443/view), Ecole Polytechnique & LIX
* [Gadi Taubenfeld](https://faculty.runi.ac.il/gadi/), Reichman University

<!--
## Attending via Zoom

For participants who cannot attend the workshop, in particular those affected by the situation in Israel, a [Zoom meeting](https://cnrs.zoom.us/j/93680383610?pwd=MkNhc0FFVzI3elVkSytrWFpYc2RxQT09) will be improvised as a degraded experience.

* Meeting ID: 936 8038 3610
* Passcode: 82DbPE
-->

## Program

* 9:00-9:45: Hagit Attiya, Technion
    <details>
    <summary><a href="static/attiya.pdf">Faithful Simulation of Randomized BFT Protocols on Block DAGs</a> (click to expand the abstract)</summary>
      <br>
      <p>
        Byzantine Fault-Tolerant (BFT) protocols that are based on Directed Acyclic Graphs (DAGs) are attractive due to their many advantages in asynchronous blockchain systems. Many DAG-based BFT protocols rely on randomization, since they are used for agreement and ordering of transaction, which cannot be achieved deterministically in asynchronous systems. Randomization is achieved either through local sources of randomness, or by employing shared objects that provide a common source of randomness, eg, common coins. This paper shows how to simulate DAG-based BFT protocols that use public coins and shared objects, like common coins. Our simulation is faithful in the sense that it precisely preserves the safety and liveness properties of the original BFT protocol, and in particular, their probability distribution.<br>

		Joint work with Constantin Enea and Shafik Nassar
      </p>
    </details>
* 9:45-10:30: Gadi Taubenfeld, Reichman University
    <details>
    <summary>Reaching Consensus in Weak Models (click to expand the abstract)</summary>
      <br>
      <p>
        I will present several results for the consensus and mutual exclusion problems in weak shared memory models (fully anonymous systems and contention-related crash failures) and discuss how formal methods can help us achieve such results.
      </p>
    </details>
* --Coffee Break--
* 10:50-11:35: Alexey Gotsman, IMDEA Software Institute
    <details>
    <summary><a href="static/gotsman.pdf">Synchronizer - a recipe for building correct algorithms under partial synchrony</a> (click to expand the abstract)</summary>
      <br>
      <p>
        Due to the FLP impossibility result, consensus protocols usually guarantee liveness only when the network is synchronous, as formalized by the partial synchrony model. To this end, the protocols are structured into a sequence of views where a dedicated leader drives the protocol towards a decision. However, synchronizing processes in the same view is challenging and can be a source of subtle bugs. I will present a formal abstraction of a synchronizer, which encapsulates the required functionality and thereby simplifies the design of consensus protocols under partial synchrony and their proofs of correctness. Synchronizers can be used in settings with either crashes or Byzantine faults. In the talk I will illustrate their use by showing how to achieve consensus liveness in the presence of crash faults and intermittently connected channels - a setting often occurring in practical cloud deployments.
      </p>
    </details>
* 11:35-12:20: Karine Altisen, University of Grenoble & Verimag
    <details>
    <summary><a href="static/altisen.pdf">PADEC - Interactive Proof for Self-Stabilizing Algorithms</a> (click to expand the abstract)</summary>
      <br>
      <p>
        PADEC is a framework to build certified proofs of self-stabilizing algorithms using the Coq proof assistant. The framework includes the definition of the computational model, tools for time complexity and composition of algorithms, lemmas for common proof patterns and case studies. A constant purpose was to convince the designers that what we formally prove using PADEC is what they expect by using definitions that are (syntactically) as close as possible to their usual definitions.
      </p>
      <p>
This talk is a summary of the libraries developed in PADEC.
      </p>
    </details>
* --Lunch Break--
* 14:00-14:45: Manuel Bravo, Informal Systems
    <details>
    <summary><a href="static/bravo.pdf">Formal modeling at Informal Systems</a> (click to expand the abstract)</summary>
      <br>
      <p>
        In this talk, I will present how we use formal methods at Informal Systems. In particular, I will talk about formal modeling and Quint, a new specification language that combines the robust theoretical basis of the Temporal Logic of Actions (TLA) with state-of-the-art static analysis and development tooling. I will present several examples in which formal modeling proved to be useful in the software development process, and the challenges of using formal methods at Informal Systems.
      </p>
    </details>
* 14:45-15:30: Rotem Oshman, Tel Aviv University
    <details>
    <summary>Distributed Certification (click to expand the abstract)</summary>
      <br>
      <p>
        In distributed certification, our goal is to certify that a network has a certain desired property - e.g., the network is connected, or the internal states of its nodes encode a valid spanning tree of the network. To this end, we store a certificate at each node, and the nodes can then interact with one another in order to decide whether to accept or reject the certificates. Our goal is to minimize the length of the certificates, the number of rounds the nodes spend interacting with one another, and the amount of communication.
In this talk I will briefly survey the area of distributed certification, and then discuss some recent research directions in the area of distributed certification, such as  adding privacy requirements and introducing computational assumptions. I will also discuss some potential areas where I believe formal methods can help us "certify the certification".
      </p>
    </details>
* --Coffee Break--
* 16:00-16:30: Louis Penet de Monterno, École Polytechnique & LIX
    <details>
    <summary><a href="static/penet.pdf">Formal Verification of a Firing Algorithm</a> (click to expand the abstract)</summary>
      <br>
      <p>
        We consider a distributed system that operates with synchronized rounds,
but with no guarantee that all agents start in the same round.
We introduce the mod P-synchronization problem, which is a weakening of the firing squad problem:
all agents must eventually send a certain signal - called firing - not at the same round, but at rounds that are equal modulo P.
We introduce an algorithm solving this problem, while tolerating a dynamic communication network.
However, this algorithm is highly combinatorial and its proof is error-prone.
To increase our confidence in the correctness of our result, we provided a formal proof written with the Isabelle proof assistant.
      </p>
    </details>
* 16:30-17:15: Ali Ebnenasir, Michigan Technological University
    <details>
    <summary><a href="static/ebnenasir.pdf">Topology and Property-Specific Verification and Synthesis of Parameterized Distributed Protocols</a> (click to expand the abstract)</summary>
      <br>
      <p>
        Verification and Synthesis (V&S) of Parameterized Distributed Protocols (PDPs) are undecidable problems, in general. To get around this undecidability result, many methods focus on specific families of protocols and/or devise semi-algorithms for V&S of PDPs with an arbitrary topology and for general safety and liveness properties. Most of such methods create an abstract model and prove its correctness, which implies the correctness of the PDP. However, the construction of abstract models by itself is a tedious task, sometimes due to assuming that the topology of the PDP is arbitrary and the property of interest for verification could be anything. In this talk, I will present a novel topology and property-specific method for V&S of PDPs, where instead of building abstract models, we identify local characterization of global failures (e.g., deadlocks and livelocks) in the local state space of template processes. Ideally, if such local characterizations are necessary and sufficient (for the existence of global failures), then detecting them can be done locally. To mitigate the V&S problem further, we focus on identifying such local characterizations in PDPs with elementary topologies (e.g., ring, tree, mesh). I will also discuss the problem of correctness-preserving composition of PDPs with elementary topologies towards synthesizing more complicated topologies. Further, I will show how local characterizations of global deadlocks and livelocks can be useful in V&S of self-stabilizing PDPs.
      </p>
    </details>
* 17:15-18:00: Pierre Fraigniaud, CNRS & IRIF
    <details>
    <summary><a href="static/fraigniaud.pdf">Decentralized Asynchronous Crash-resilient Runtime Verification</a> (click to expand the abstract)</summary>
      <br>
      <p>
        Runtime verification is a lightweight method for monitoring the formal specification of a system during its execution. It has recently been shown that a given state predicate can be monitored consistently by a set of crash-prone asynchronous distributed monitors observing the system, only if each monitor can emit verdicts taken from a large enough finite set. We revisit this impossibility result in the concrete context of linear-time logic (LTL) semantics for runtime verification, that is, when the correctness of the system is specified by an LTL formula on its execution traces. First, we show that monitors synthesized based on the 4-valued semantics of LTL (RV-LTL) may result in inconsistent distributed monitoring, even for some simple LTL formulas. More generally, given any LTL formula φ, we relate the number of different verdicts required by the monitors for consistently monitoring φ, with a specific structural characteristic of φ called its alternation number. Specifically, we show that, for every k≥0, there is an LTL formula φ with alternation number k that cannot be verified at runtime by distributed monitors emitting verdicts from a set of cardinality smaller than k+1. On the positive side, we define a family of logics, called distributed LTL (abbreviated as DLTL), parameterized by k≥0, which refines RV-LTL by incorporating 2k+4 truth values. Our main contribution is to show that, for every k≥0, every LTL formula φ with alternation number k can be consistently monitored by distributed monitors, each running an automaton based on a (k+4)-valued logic taken from the DLTL family.
      </p>
    </details>

## Summary of the workshop

Distributed algorithms is an active research field; their applications range
from Internet applications over cloud computing to safety-critical control
systems. Whereas many applications are of critical importance, the correctness
of distributed algorithms is usually based on very subtle mathematical
arguments. Consequently, one easily can make mistakes with hand-written proofs,
which reduces the trust in the correctness of these systems.

In the last decades, formal methods were proven to be useful for the
verification of many hardware and software systems. For distributed algorithms,
the application of formal methods was limited: formal methods have been used
for finding bugs in distributed algorithms, and to a much smaller extent formal
methods were used in computer-aided verification of simple distributed
algorithms. However, to verify more involved distributed algorithms, one cannot
easily apply existing verification tools. To be eventually able to do this, an
interdisciplinary effort from the concerned fields of formal methods, logic in
computer science, and distributed algorithm theory is required.

The topics of interest for the FRIDA workshop include the following topics, as
they apply to distributed algorithms and systems:

* formal modeling
* model checking
* interactive theorem proving
* parameterized model checking
* integration of different verification techniques
* benchmarking
* synthesis
* run-time verification
* testing
* invariant inference

## Organizers

### Main organizers
* [Marijana Lazić](https://www.cs.cit.tum.de/tcs/personen/marijana-lazic/#c26286)
* [Stephan Merz](https://members.loria.fr/Stephan.Merz/)

### With support of
* [Giuliano Losa](https://www.losa.fr/)
* Igor Konnov
* [Swen Jacobs](https://cispa.de/en/people/swen.jacobs)
* Joseph Widder

## Previous editions

Starting a productive dialogue between distributed algorithms and verification
communities was the goal of a successful [Dagstuhl Seminar “Formal Verification
of Distributed Algorithms”](https://www.dagstuhl.de/en/program/calendar/semhp/?semnr=13141)
which was held in April 2013. During this seminar,
the participants agreed that a series of workshops should be held in order to
strengthen the community that does research on these issues.

The [1st workshop on Formal Reasoning in Distributed
Algorithms](https://easychair.org/smart-program/VSL2014/FRIDA-index.html) took
place in Vienna as part of the Vienna Summer of Logic’14 and Federated Logic
Conference’14. The [2nd FRIDA
workshop](http://discotec2015.inria.fr/workshops/frida-2015/) took place in
Grenoble as part of FORTE’15. The [3rd FRIDA
workshop](https://forsyte.at/events/frida2016/) was organized in Marrakech as
part of NETYS’16. The [4th FRIDA
workshop](https://forsyte.at/events/frida2017/) took place in Vienna as part of
DISC 2017. The [5th FRIDA workshop](https://forsyte.at/events/frida2018/) was
co-located with CAV 2018, which was held as part of the Federated Logic
Conference (FLoC). The [6th
workshop](https://team.inria.fr/veridis/events/frida2019/) was co-located with
DISC 2019 in Budapest, Hungary. Finally, [FRIDA 2020](https://frida2020.galois.com/) and [FRIDA 2021](https://frida-2021.github.io) took place as online workshops at QONFEST 2020 and DISC 2021, respectively.
[FRIDA 2022](https://frida-2022.github.io) was organize with FLoC 2022 and took place in Haifa.
