---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

# The 10th Workshop on Formal Reasoning in Distributed Algorithms

Date: Monday October 9th, 2023
Location: L'Aquila, Italy

The workshop is organized as part of [DISC 2023](http://www.disc-conference.org).

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
## News

* July 18th: initial website created!
-->

## Program

* 9:00-9:45:  Rotem Oshman, Tel Aviv University
    <details>
    <summary>Distributed Certification (click to expand the abstract)</summary>
      <br>
      <p>
        In distributed certification, our goal is to certify that a network has a certain desired property - e.g., the network is connected, or the internal states of its nodes encode a valid spanning tree of the network. To this end, we store a certificate at each node, and the nodes can then interact with one another in order to decide whether to accept or reject the certificates. Our goal is to minimize the length of the certificates, the number of rounds the nodes spend interacting with one another, and the amount of communication.
In this talk I will briefly survey the area of distributed certification, and then discuss some recent research directions in the area of distributed certification, such as  adding privacy requirements and introducing computational assumptions. I will also discuss some potential areas where I believe formal methods can help us "certify the certification".
      </p>
    </details>
* 9:45-10:30: Gadi Taubenfeld, Reichman University
    <details>
    <summary>TBA (click to expand the abstract)</summary>
      <br>
      <p>
        TBA
      </p>
    </details>
* --Coffee Break--
* 11:00-11:45: Alexey Gotsman, IMDEA Software Institute
    <details>
    <summary>Synchronizer - a recipe for building correct algorithms under partial synchrony (click to expand the abstract)</summary>
      <br>
      <p>
        TBA
      </p>
    </details>
* 11:45-12:30: Karine Altisen, University of Grenoble & Verimag
    <details>
    <summary>TBA (click to expand the abstract)</summary>
      <br>
      <p>
        TBA
      </p>
    </details>
* --Lunch Break--
* 14:00-14:45: Manuel Bravo, Informal Systems
    <details>
    <summary>TBA (click to expand the abstract)</summary>
      <br>
      <p>
        TBA
      </p>
* 14:45-15:30: Hagit Attiya, Technion
    <details>
    <summary>Faithful Simulation of Randomized BFT Protocols on Block DAGs (click to expand the abstract)</summary>
      <br>
      <p>
        Byzantine Fault-Tolerant (BFT) protocols that are based on Directed Acyclic Graphs (DAGs) are attractive due to their many advantages in asynchronous blockchain systems. Many DAG-based BFT protocols rely on randomization, since they are used for agreement and ordering of transaction, which cannot be achieved deterministically in asynchronous systems. Randomization is achieved either through local sources of randomness, or by employing shared objects that provide a common source of randomness, eg, common coins. This paper shows how to simulate DAG-based BFT protocols that use public coins and shared objects, like common coins. Our simulation is faithful in the sense that it precisely preserves the safety and liveness properties of the original BFT protocol, and in particular, their probability distribution.

		Joint work with Constantin Enea and Shafik Nassar
      </p>
    </details>
* --Coffee Break--
* 16:00-16:30: Louis Penet de Monterno, École Polytechnique & LIX
    <details>
    <summary>TBA (click to expand the abstract)</summary>
      <br>
      <p>
        TBA
      </p>
    </details>
* 16:30-17:15: Ali Ebnenasir, Michigan Technological University
    <details>
    <summary>TBA (click to expand the abstract)</summary>
      <br>
      <p>
        TBA
      </p>
    </details>
* 16:30-17:15: Pierre Fraigniaud, CNRS & IRIF
    <details>
    <summary>TBA (click to expand the abstract)</summary>
      <br>
      <p>
        TBA
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
