---
layout: archive
title: ""
permalink: /projects/
author_profile: true
---

<h2>Georgia Institute of Technology, Atlanta, Georgia</h2>

<details>
	<summary>Qubit Allocation Policies with Variation Awareness</summary>
    <h6><i>Instructor: Prof. Moin Qureshi, School of ECE - ECE 8853: Introduction to Quantum Computing, Spring 2019</i></h6>
    <ul>
        <li>There's a technological gap between the quantum software and hardware for NISQ computers, which makes qubit mapping a challenge as two logically coupled qubits need to be optimally physically mapped to perform operations, and this has to be done with the minimum number of SWAP operations. To overcome this, a SWAP-based BidiREctional heuristic search algorithm, named SABRE is used, that finds the best initial mapping of the qubits that will give the least number of SWAPs.</li> 
        <li>However, SABRE doesn't take into account the imperfect links and qubit error rates as they exist on real quantum computers (IBMQ16), and SABRE was hence modified to accommodate variation-aware qubit allocation and movement. To implement this, variation-aware scheduler was designed that in addition to the SWAPs given by baseline SABRE, schedules the single-qubit instructions that use the same qubits as the CNOTs alongwith any independent instructions that are not affected by the CNOTs and possibly resulting SWAPs. To maintain a list of logical qubit mappping, a remap table structure is designed that tracks which physical qubit the logical qubit is mapped to. The cost function that determines the best possible SWAP combination is modified to take into account the error rates of the links. </li>
        <li>Across 7 quantum workloads, it was observed that the Probability of Successful Trial (PST) increased by an average of 14% whereas the number of SWAPs for that algorithm reduced by an average of 8%. </li>
    </ul>
</details>

<details>
	<summary>Information Security</summary>
    <h6><i>Instructor: James Cannady, Georgia Tech Research Institute</i></h6>
    <h6>CS 6235: Introduction to Information Security, Spring 2019</h6>
    <ul>
        <li>Implemented a stack buffer overflow attack that invokes a new shell by manipulating the list of integers to be sorted.</li>
        <li>Performed malware analysis for 4 types of malware by reading into its registry contents.</li>
        <li>Implemented RSA encryption and decryption algorithm. Explored security flaws due to faulty random number generator used for key generation, and effect of small exponent for broadcast RSA attack.</li>
        <li>Implemented XSRF attack, DOM-based XSS attack and SQL injection attack on web pages.</li>
    </ul>
</details>

<details>
    <summary>Relaxing PIM Synchronization Constraints</summary>
    <h6><i>Instructor: David Devecsery, College of Computing</i></h6>
    <h6>ECE 8803: Memory Models, Fall 2018</h6>
    <ul>
        <li>Graph processing is one of the most widely used workloads in high performance computing, which is highly limited by the memory wall and, traditional architectural improvements on parallelism do not help improving the performance of graph applications as data accesses here are very irregular. Architects have proposed to utilize Hybrid Memory Cube (HMC) to move computation in/near memory called Processing in Memory (PIM).</li>
        <li>The synchronization overheads are here relaxed for the popular Gather-Apply-Scatter graph processing paradigm by relaxing the memory consistency requirements using a novel technique based on “colored” barriers, which is determined by some pre-processing of a graph snapshot. Weaker memory consistency semantics enable us to extract performance and yet provide an illusion of sequential consistency given some semantic constraints are met. </li>
        <li>Our approach shows a speedup of over ∼6% for highly-connected and ∼30% for sparsely-connected graphs over the baseline Gather-Apply-Scatter implementation with minimum modifications to existing hardware.</li>
    </ul>
</details>

<details>
    <summary>GPU Architectures</summary>
    <h6><i>Instructor: Prof. Sudhakar Yalamanchili, School of ECE</i></h6>
    <h6>ECE 8823: GPU Architectures, Spring 2018</h6>
    <ul>
        <li>Implemented CUDA kernel for 2D convolution to perform image blur on RGB image with both constant and shared memory. </li>
        <li>Implemented CUDA kernels to implement the computation graph of a convolutional neural network to perform image recognition on a gray-scale image.</li>
        <li>Implemented PDOM stack algorithm for branch divergence in GPUs on HARP emulator for divergent and nested divergent warps, and divergent loops, using SPLIT/JOIN in assembly language.</li>
    </ul>
</details>

<details>
    <summary>Analysis of EM Emanations from Cache Side-Channel Attacks on IoT Devices</summary>
    <h6><i>Instructor: Hyesoon Kim, College of Computing</i></h6>
    <h6>CS 7290: Advanced Microrchitecture, Fall 2017</h6>
    <ul>
        <li>Implemented FLUSH+RELOAD cache side-channel attack to demonstrate proof-of-concept on GnuPG RSA and bitcnts (MiBench).</li>
        <li>Observed prominent loops due to probing in frequency-time spectra of application with FLUSH+RELOAD.</li>
    </ul>
</details>

<details>
    <summary>FPGA Systems Design using Verilog</summary>
    <h6><i>Instructor: Timothy Brothers, Georgia Tech Research Institute</i></h6>
    <h6>ECE 8813: Advanced Digital Design with Verilog, Spring 2017</h6>
    <ul>
        <li>Designed and implemented various FPGA-based system controllers for GPS, VGA-Serial convertor and irrigation systems in Quartus. </li>
        <li>Implemented image transpose and Sobel operator based edge detection on a grayscale image using an FPGA.</li>
    </ul>
</details>

<details>
    <summary>Polish Expression based Floorplanning : Simulated Annealing</summary>
    <h6><i>Instructor: Prof. Sung-Kyu Lim, School of ECE</i></h6>
    <h6>ECE 6133: Physical Design Automation, Fall 2016</h6>
    <ul>
        <li>Created a simulator to perform optimized floorplanning on any given list of hard blocks based on a simulated annealing approach minimizing both area and half perimeter wire length. </li>
        <li>In order to create more room for optimization, the * and + operators in the initial Polish expression were taken randomly. Data structures were created to model the Polish expression and the slicing tree that take into account all internal nodes, including left, right and parent nodes, facilitating fast development of advanced algorithms, and the graphics was created using OpenGL.The cooling rate, initial temperature, cost function and stopping conditions were set based on the saturation observed after multiple runs of simulated annealing. </li>
        <li>Apart from the conventional M1, M2 and M3 moves of simulated annealing, an M4 move was introduced to rotate the operand modules at lower temperatures, easing the path to reach the local minima. The Stockmeyer algorithm applied after the simulated annealing had almost no change as the M4 move was either very close or already at the most optimal solution.</li>
        <li>Overall, it was observed that an average of 65% HPWL reduction, 90% chip area reduction and 80% chip utilization was achieved after testing multiple differently sized circuits on the designed simulator.</li>
    </ul>
</details>

<details>
    <summary>Handling C++ STL Libraries</summary>
    <h6><i>Instructor: Prof. George P. Riley, School of ECE</i></h6>
    <h6>ECE 6122: Advanced Programming Techniques, Fall 2016</h6>
    <ul>
        <li>Implemented 2D image Fourier Transform using MPI and pthreads with barrier.</li>
        <li>Using the GMP library, performed RSA encryption, decryption and breaking using Pollard rho algorithm for factorization.</li>
        <li>Explored the OpenGL library by creating a rotating icosahedron of varying vertices.</li>
        <li>Created a custom library identical to the vector STL library containing corresponding functions.</li>
        <li>Implemented Mandelbrot set using OpenGL for graphics and pthreads for speed improvement with zoom function.</li>
    </ul>
</details>

<details>
    <summary>Out-of-order Superscalar Processor using Tomasulo Algorithm </summary>
    <h6><i>Instructor: Prof. Tom Conte, School of ECE</i></h6>
    <h6>ECE 6100: Advanced Computer Architecture, Spring 2016</h6>
    <ul>
        <li>Designed a 5-stage pipeline structure with Fetch, Dispatch, Scheduling, Execute and State Update. </li>
        <li>Implemented two exception handling schemes: ROB with bypass and Checkpoint Repair. </li>
        <li>Experimented successfully on multiple setups. </li>
    </ul>
</details>

<details>
    <summary>Approximation on On-Chip Networks for Mitigation of Memory and Bandwidth Walls</summary>
    <h6><i>Instructor: Tushar Krishna, School of ECE</i></h6>
    <h6>ECE 8823: Interconnection Networks, Spring 2016</h6>
    <ul>
        <li>Developed a novel approach to solve the tradeoff problem of limited off-chip bandwidth and long access latency in CMPs by implementing approximation on on-chip networks.</li>
        <li>Based on Rollback-Free Value Prediction approximation technique, which manipulates safe-to-approximate loads in LLC misses.</li>
        <li>Here, safe-to-approximate loads are manipulated by the approximator both at the network interface and in a router using a drop rate parameter, which decides the fate of a traversing flit – drop or continue.</li>
        <li>Achieved up to 10% power efficiency and 50% latency improvement for an 8x8 mesh topology at a cost of 80% accuracy with a negligible area overhead.</li>
    </ul>
</details>

<details>
    <summary>SRAM Memory System and Arithmetic Unit</summary>
    <h6><i>Instructor: Prof. Saibal Mukhopadhyay, School of ECE</i></h6>
    <h6>ECE 6130: Advanced VLSI Systems, Fall 2015</h6>
    <ul>
        <li>Designed a 50 nm technology based adder system interfaced with 16x32 SRAM array to perform sequential reads and accumulation.</li>
        <li>Achieved full functionality in post-layout simulation and compared its performance against pre-layout simulation.</li>
        <li>The post-layout design with its extracted parasitics achieved a total power consumption of 470 uW with an SRAM array area efficiency of 63.37% when operated on a nominal supply voltage of 800 mV and frequency of 1 GHz.</li>
        <li>In comparison with other teams, our design had capabilities of working at frequencies upto 2.93 GHz even at nominal voltage.</li>
    </ul>
</details>

     

<h2>VES Institute of Technolgy, University of Mumbai, India</h2>

<details>
    <summary>An Innovative Approach to Location based Services and Traffic Management System</summary>
    <h5><a href="https://www.youtube.com/embed/ftGNE3rXwQI">Project Demo</a> &nbsp; <a href="https://www.youtube.com/embed/Ux3pjuXfrpw">On-field Demo</a></h5>
    <h6><i>Instructor: Mr. Hardik Shah, VES Institute of Technology</i></h6>
    <h6>B.E. Final Year Project, 2014 - 2015</h6>
    <ul>
        <li>Built a positioning and navigation system based on the communication between the RF transmitters present on the road and the RF receiver present in the vehicle without using the Internet or GPS, based on offline maps.</li>
        <li>Worked on TI's ARM Cortex M4 Tiva controller and CC2530 SoC for RF communication.</li>
        <li>Developed touch screen GUI and incorporated features such as emergency services and vehicle tracking.</li>
        <li>Implemented the system throughout the college campus.</li>
    </ul>
</details>

<details>
    <summary>Kindle for the Blind</summary>
    <h5><a href="https://www.youtube.com/embed/ZGs2-nnhLTY">Project Demo</a></h5>
    <h6><i>Mentor: Mr. Hardik Shah, VES Institute of Technology</i></h6>
    <h6>Texas Instruments Innovation Challenge, India Analog Design Contest 2014</h6>
    <ul>
        <li>Funded by Texas Instruments India (out of 1754 proposals from 321 colleges across India). Competed as semi-finalists in the competition.</li>
        <li>Built a TI's MSP430F5659 microcontroller based device to take voice input from a visually impaired user of the eBook name and display the eBook on the prototypic LED matrix display by loading it from the flash drive containing the eBooks stored in a .txt format.</li> 
    </ul>
</details>