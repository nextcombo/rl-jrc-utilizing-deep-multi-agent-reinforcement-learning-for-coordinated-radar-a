# [RL+JRC] Utilizing Deep Multi-Agent Reinforcement Learning for Coordinated Radar and Communication Scheduling [with Python code attached]

Introduction 
In the future, ELF vehicles will need to perform multiple tasks to promote their ultimate goal of safe navigation, including sensor and perception, positioning, obstacle map, and path finding. In collaborative driving environments, a large amount of data must be transmitted; communication can occur between vehicles (V2 V) or between vehicles and infrastructure (V2X). With the commercialization of 5G communication technology and associated with higher frequency (e.g. millimeter wave bands), interference from radar waves has become possible. 
The issue of jointly operating radar and communication functions within the same frequency range is known as Joint Radar Communication (JRC) or Communication and Radar Spectrum Sharing (CRSS). The implementation methods of JRC systems have been reviewed by [1] and [2]. These methods can generally be divided into three different approaches: using communication signals for object detection, modulating communication signals onto radar pulses, and time-division between radar operation and communication. 
More traditional time-division methods use fixed schedules alternating between radar and communication [2] and [3]. In contrast, [4] proposed a learning-based method for automotive use. The main advantage of this method is that the communication system can learn to respond to instantaneous changes in environmental conditions, which may require increasing the radar operation frequency to support safe navigation. 
Another challenge related to data communication in autonomous vehicles is the high data rate and freshness of sensory information required for safe navigation, as well as the low latency internet connection needed for the onboard entertainment system. Autonomous vehicles typically are equipped with a set of sensors to reliably perceive their environment: cameras, lidar, radar, ultrasonic sensors, inertial measurement units, and satellite-based positioning systems such as GPS. Exosensing sensors generate a large amount of data due to their multidimensional nature [5]. This requires timely transmission to surrounding vehicles or infrastructure in a collaborative driving setting.
The traditional performance metrics for data communication, such as throughput or latency, may be useful for in-vehicle entertainment systems. However, they may not be sufficient to evaluate the communication of haptic data in collaboration. They require immediate response scenarios. The author presents an example in [6] where packets containing old information might be useless even with very small delays. In automotive environments, a more suitable metric for measuring the timeliness of communication is Information Age (AoI), defined as the duration since the last received packet was generated [7].
In this paper, we consider a joint approach that minimizes AoI and maintains radar responsiveness through temporal segmentation. We consider both single-agent and multi-agent scenarios. The main considerations that prompt us to pose and solve problems are as follows:
1) Environmental awareness - The agent must be able to adjust its radar detection usage to cope with the increased importance of radar.
2) Urgency relevance - Autonomous vehicles can transmit several types of data. Our JRC system should prioritize the communication of more important data.
3) Low prior knowledge - The JRC system should require minimal prior knowledge about the vehicle's environment, the systems it operates on, and the nature of the data it wants to communicate.
4) Decentralized execution - Vehicles in a multi-agent environment should be able to make decisions in a decentralized manner after training.
This work is an important improvement and extension of the time-based JRC method proposed in literature [4] and [8]. Our contributions are as follows:
1) A framework for managing multiple data queues for individual vehicle agents, each class representing different levels of urgency for different data groups. We formulate this problem as a Markov Decision Process (MDP).
2) A deep reinforcement learning-based time-based method for jointly coordinating radar operations by training agents to minimize the AoI of transmitted data.
3) A more generalized formula for multi-agent systems simulating real-world vehicle communication scenarios. This problem is described as a Partially Observable Markov Game (POMG), which is a generalization of MDPs.
4) In multi-agent systems, the use of Media Access Control (MAC) technology combined with deep reinforcement learning methods to train agents.
Article illustrations
Conclusion
We considered the Joint Radar Communications (JRC) problem for autonomous vehicles, aiming to jointly optimize radar operations and the information age (AoI) of multiple data queues through finding real-time time-division strategies. By reviewing contemporary literature in automotive sensors and perception, combined with modern understanding of road traffic safety, we established that the JRC dispatch strategy module can be integrated into the automotive perception system, and how wise scheduling of radar sensing can support road safety objectives. Our framework's problem is presented as a Markov Decision Process (MDP), and we propose a generalized Partially Observable Markov Game (POMG) system composition for multiple decentralized vehicles. We contribute theoretical analysis and solve MDP and POMG using deep reinforcement learning. Experimental results show that the selected deep reinforcement learning method outperforms all baseline algorithms, despite having little information about the environment. The findings also reveal two discoveries. First, our proposed convolutional neural network (CNN) architecture is more effective in extracting features from raw representations of data queues. Second, entropy regularization enables agents in POMG to achieve better performance by exploring the state-action space more effectively. Future work may consider methods for implicit learning to adapt to changing environmental parameters; this could include more realistic communication request bursts and more complex changes in channel conditions.
End

## Images

![[RL+JRC] Utilizing Deep Multi-Agent Reinforcement Learning for Coordinated Radar and Communication Scheduling [with Python code attached]](01.jpg)
![[RL+JRC] Utilizing Deep Multi-Agent Reinforcement Learning for Coordinated Radar and Communication Scheduling [with Python code attached]](02.jpg)
![[RL+JRC] Utilizing Deep Multi-Agent Reinforcement Learning for Coordinated Radar and Communication Scheduling [with Python code attached]](03.jpg)
![[RL+JRC] Utilizing Deep Multi-Agent Reinforcement Learning for Coordinated Radar and Communication Scheduling [with Python code attached]](04.jpg)
![[RL+JRC] Utilizing Deep Multi-Agent Reinforcement Learning for Coordinated Radar and Communication Scheduling [with Python code attached]](05.jpg)
![[RL+JRC] Utilizing Deep Multi-Agent Reinforcement Learning for Coordinated Radar and Communication Scheduling [with Python code attached]](06.jpg)
![[RL+JRC] Utilizing Deep Multi-Agent Reinforcement Learning for Coordinated Radar and Communication Scheduling [with Python code attached]](07.jpg)
![[RL+JRC] Utilizing Deep Multi-Agent Reinforcement Learning for Coordinated Radar and Communication Scheduling [with Python code attached]](08.jpg)
![[RL+JRC] Utilizing Deep Multi-Agent Reinforcement Learning for Coordinated Radar and Communication Scheduling [with Python code attached]](09.jpg)
![[RL+JRC] Utilizing Deep Multi-Agent Reinforcement Learning for Coordinated Radar and Communication Scheduling [with Python code attached]](10.jpg)
![[RL+JRC] Utilizing Deep Multi-Agent Reinforcement Learning for Coordinated Radar and Communication Scheduling [with Python code attached]](11.jpg)
![[RL+JRC] Utilizing Deep Multi-Agent Reinforcement Learning for Coordinated Radar and Communication Scheduling [with Python code attached]](12.jpg)

<!-- PAYMENT_BLOCK -->

## Get this dataset

- Payment link (Stripe): [Buy now](https://buy.stripe.com/3cs8yP7sY87d0vu9AB)
- Payment QR code: ![Payment QR code](pay.png)

<!-- /PAYMENT_BLOCK -->
