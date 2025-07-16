Design and Validation of a Hybrid MPPT Algorithm for Photovoltaic System Using Interleaved Boost Converter
ID Number: 9715

Authors description: 

Luis Enrique Hernández Aguilar (Member, IEEE) Electronics engineer graduated from the Instituto Superior de Irapuato with a specialty in power electronics in 2024. He is currently a master’s student in power electronics engineering at the same institute

Gerardo Vázquez Guzmán (Senior Member, IEEE) was born in Mexico, on September 24, 1977. He received the Ph.D. degree in electrical engineering from the Technical University of Catalonia, in 2013. 

Panfilo Raymundo Martínez Rodríguez (Senior Member, IEEE) received the Ph.D. degree in applied science from Instituto Potosino de Investigacion Cientifica y Tecnologica A.C. IPICYT, San Luis Potosi, Mexico, in 2007. 

Dalyndha Aztatzi Pluma She was born in Mexico on November 10, 1985. She received the Ph.D. degree in chemical engineering from the Technological Institute of Celaya, in 2017.

The MPPT algorithms implemented in the Matlab environment are detailed below. These can be reproduced in the software console when acting within the Simulink environment when connected to PV and electrical operating blocks.  This is dependent on the proper definition of the input parameters, such as the voltage between the PV panel terminals and the PV panel output current.

The MPPT algorithms allow tracking the maximum power point in a PV system, since the operating point depends on environmental conditions it is necessary to ensure that it is operated consistently at the best possible operating point, which represents a greater economic and energetic benefit.

The Hill Climbing, Perturb & Observe algorithms belong to a subgroup called trial and error, although their tracking accuracy is lower than the rest, they are easy to implement. In these the MPP is tracked by varying the duty cycle of the converter based on power and voltage conditions, i.e. if they increase or decrease.

The Incremental Conductance algorithm belongs to the mathematical calculation subgroup, the MPP is tracked by varying the duty cycle of the converter according to the calculation of the incremental conductance and the instantaneous conductance, and the relationship between these two parameters.

The Particle Swarm Optimization algorithm is considered an intelligent algorithm that allows tracking the MPP even under shading conditions, which the previous algorithms cannot do correctly. In this algorithm, thirteen fixed duty cycles are defined, and the power of each cycle is calculated, at the end only the duty cycle with which the highest magnitude of power was obtained is kept.

The proposed hybrid algorithm based on the Particle Swarm Optimization and Perturb & Observe algorithms operates in such a way that seven fixed duty cycles are defined, optimizing the response time, once the duty cycle that generated the maximum power is measured it is maintained and the Perturb and Observe algorithm comes into operation with a finer duty cycle increment tracking the MPP more efficiently and with less oscillation.
